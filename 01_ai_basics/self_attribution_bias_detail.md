# AIの自己帰属バイアスと自己監視の限界

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L1-ATTR-DETAIL |
| Version（バージョン） | 0.1 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L1 一覧](./README.md) / [簡易版](./self_attribution_bias_basic.md) / [AIへの頼み方](./how_to_ask_ai.md) / [AI利用時の安全ルール](./ai_safety_basic.md) |

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Terminology（用語）](#3-terminology用語)
4. [Observed Behavior（観測されている挙動）](#4-observed-behavior観測されている挙動)
5. [Context Attribution（文脈と帰属）](#5-context-attribution文脈と帰属)
6. [On-Policy / Off-Policy Evaluation](#6-on-policy--off-policy-evaluation)
7. [Practical Risks（実務上のリスク）](#7-practical-risks実務上のリスク)
8. [Countermeasures（対策）](#8-countermeasures対策)
9. [Relationship to SCAO](#9-relationship-to-scao)
10. [Limitations（適用範囲と限界）](#10-limitations適用範囲と限界)
11. [References（参考文献・公式情報）](#11-references参考文献公式情報)
12. [Change History（変更履歴）](#12-change-history変更履歴)

## 1. Purpose（目的）

AIが自分の出力を評価するときに生じる「自己帰属バイアス」と、AIによる自己監視の限界を理解する。
そのうえで、生成と評価を同一AIで自己完結させないための、実務寄りの対策を身につける。

## 2. Target Audience（対象読者）

- AIにコードや作業結果のレビュー・承認をさせている人
- AIエージェントの半自動ループを組みたい初学者
- 簡易版を読み、より深い背景と対策を知りたい人

先に [簡易版](./self_attribution_bias_basic.md) を読んでおくと理解しやすい。

## 3. Terminology（用語）

以下は関連するが同じではない。完全な同義語として扱わない。

- Self-Attribution Bias（自己帰属バイアス）
  - ある対象が「自分の出力」として帰属（提示）されたとき、他者由来の同一対象より甘く評価する傾向。評価対象の中身は同じで、「誰の出力として提示されたか」だけが異なる点が特徴。
- Self-Preference Bias（自己選好バイアス）
  - 自身または同系統（同じモデルファミリー）の生成物を、相対的に高く評価する傾向。
- Self-Justification Bias（自己正当化バイアス）
  - 過去の判断や回答を維持・正当化し、誤りやリスクを過小評価する関連挙動を説明する表現。

この学習用資料では、研究で中心的に扱われる「自己帰属バイアス」を主軸に置き、自己選好・自己正当化は関連概念として区別して扱う。

## 4. Observed Behavior（観測されている挙動）

一次資料（Khullar et al., 2026, arXiv:2603.04582）では、次のような挙動が報告されている。

- 同じ行動（コードやツール操作）でも、それが「自分が直前に生成したもの」として暗黙に提示されると、リスクを低く・正しさを高く評価しやすい。
- この効果は、作者を明示的に「同じモデルだ」と述べただけでは強く出ない。むしろ、会話構造上「直前のアシスタント発話」として暗黙に自分の出力になっているときに強く出る。
- ある設定では、プロンプトインジェクション後のコード修正を、自己帰属の状況では約5倍承認しやすくなったと報告されている。

重要な注意（断定しない）：

- これは「AIに人間と同じ自我がある」ことを意味しない。
- 「AIが意図的に嘘をつく」ことを示すものでもない。
- 「すべてのAIが必ず自分の出力を正当化する」わけではない。
- あくまで、複数モデル・複数データセットで観測された評価傾向である。

## 5. Context Attribution（文脈と帰属）

- 帰属とは、「その出力が誰のものとして提示されているか」を指す。
- 明示的帰属：プロンプトで「これはあなたの出力です」と書く。研究では効果は弱いとされる。
- 暗黙的帰属：会話の流れ上、直前の自分の発話が評価対象になる。研究では効果が強いとされる。
- つまり、同じ会話履歴の中で自分の出力を続けて評価させる形が、最もバイアスが出やすい。

## 6. On-Policy / Off-Policy Evaluation

- オンポリシー評価：AIが、自分が同一文脈で直前に生成した成果物を、そのまま評価する。
  - 例：あるチャットでAIにコードAを書かせ、同じチャットで「このコードAに問題はある？」と続けて聞く。
- オフポリシー評価：新しい文脈・別AI・第三者から提示された成果物として評価する。
  - 例：別のチャットを開き、「次のコードをレビューして」とコードAだけを貼って評価させる。または別のAIに評価させる。

研究では、自己帰属バイアスはオンポリシー（自分が今作ったものを評価）で最も強く、オフポリシー（他者由来として評価）では弱まる、または消えると報告されている。
このため、固定データセット（externally supplied）だけで監視性能を測ると、実運用より高性能に見えてしまう危険がある。

## 7. Practical Risks（実務上のリスク）

- 生成コードのセルフレビューで、バグを見逃す。
- 危険なツール操作（削除・外部送信など）を、自ら「安全」と承認してしまう。
- 情報漏洩や破壊的処理を、低リスクと誤判定する。
- 完全自動ループにおいて、AIの自己監視が形式的なチェックに堕し、実質的に機能しなくなる。
- 固定評価では高性能に見えても、実運用（自分の出力を監視する状況）では検出力が低下する可能性。
- 同じ会話履歴にある自分の出力を再評価させると、バイアスが強まる危険。

## 8. Countermeasures（対策）

次の順序で、重ねて適用する。

1. 生成者と評価者の分離：作るAIと評価するAIの役割を分ける。
2. 文脈分離：評価は同じ会話の続きではなく、新しい文脈で行う（オフポリシー化）。
3. マルチモデル評価：異なるモデル・ベンダーのAIにも評価させる。
4. 機械的検証：テスト、静的解析、差分確認など、AIに依らない検証を併用する。
5. 人間確認ゲート：重要判断は人間が最終確認する。
6. 事前に定義された受け入れ条件：「何を満たせば合格か」を作業前に決めておく（後付けで基準を緩めない）。
7. 破壊的操作前の停止条件：commit・push・削除・外部送信などの前で必ず停止し、人間が確認する。

## 9. Relationship to SCAO

SCAOの考え方の一例として、役割ごとに担当を分ける構成がある。

| 役割 | 担当 |
|---|---|
| 調査 | Gemini |
| 設計 | ChatGPT |
| 実装 | Cursor |
| 独立レビュー | Claude |
| 最終判断 | 人間 |

これは、同一AIが「生成」と「承認」を自己完結する構造を避けるための、一つの設計である。

ただし、次も明記する。

- AIを分けるだけでは完全ではない。
- 学習データの共通性などにより、共通の誤学習や同種のバイアスは残りうる。
- テスト・差分確認・人間判断を組み合わせる必要がある。

## 10. Limitations（適用範囲と限界）

- 本文の記述は、観測された傾向に基づくものであり、すべてのモデル・状況で必ず成立する法則ではない。
- 研究は特定のモデル群・データセットでの結果であり、将来のモデルや別の設定では挙動が異なりうる。
- 対策を組み合わせても、バイアスを完全には除去できない。最後は人間の判断が必要。
- 本学習用資料は初学者向けの要約であり、原論文の主張を簡略化している。正確な条件・数値は一次資料を参照すること。

## 11. References（参考文献・公式情報）

一次資料および関連研究（arXiv はプレプリントであり、査読済み論文と断定しない。査読状況は未確認）。

| タイトル | 著者・公開主体 | 公開年 | 資料種別 | URL | 使用箇所 | 確認日 |
|---|---|---|---|---|---|---|
| Self-Attribution Bias: When AI Monitors Go Easy on Themselves | Dipika Khullar, Jack Hopkins, Rowan Wang, Fabien Roger | 2026 | arXiv プレプリント（一次資料） | <https://arxiv.org/abs/2603.04582> | 4章・5章・6章（自己帰属バイアス、暗黙的帰属、オンポリシー/オフポリシー） | 2026-07-15 |
| LLM Evaluators Recognize and Favor Their Own Generations | Arjun Panickssery, Samuel R. Bowman, Shi Feng | 2024 | arXiv プレプリント（関連研究） | <https://arxiv.org/abs/2404.13076> | 3章（自己認識と自己選好の関連） | 2026-07-15 |
| Self-Preference Bias in LLM-as-a-Judge | Koki Wataoka, Tsubasa Takahashi, Ryokan Ri | 2024 | arXiv プレプリント（関連研究） | <https://arxiv.org/abs/2410.21819> | 3章（自己選好とパープレキシティ由来の親近性） | 2026-07-15 |
| Do LLM Evaluators Prefer Themselves for a Reason? | Wei-Lin Chen, Zhepei Wei, Xinyu Zhu, Shi Feng, Yu Meng | 2025 | arXiv プレプリント（関連研究） | <https://arxiv.org/abs/2504.03846> | 7章・8章（有害な自己選好、CoTによる緩和） | 2026-07-15 |
| Self-Preference Bias in Rubric-Based Evaluation of Large Language Models | José Pombal, Ricardo Rei, André F. T. Martins | 2026 | arXiv プレプリント（関連研究） | <https://arxiv.org/abs/2604.06996> | 8章（ルーブリック評価でも自己選好が残る、アンサンブルで緩和） | 2026-07-15 |

補助資料（自己帰属バイアスを直接実証した資料ではない。監視・正直性に関する関連する公式研究記事として参照）。

| タイトル | 公開主体 | 公開年 | 資料種別 | URL | 使用箇所 | 確認日 |
|---|---|---|---|---|---|---|
| Evaluating chain-of-thought monitorability | OpenAI | 2025 | 企業公式研究記事（補助資料） | <https://openai.com/index/evaluating-chain-of-thought-monitorability/> | 7章・8章（AI監視の限界と補完手段の背景） | 2026-07-15 |
| How confessions can keep language models honest | OpenAI | 2025 | 企業公式研究記事（補助資料） | <https://openai.com/index/how-confessions-can-keep-language-models-honest/> | 8章（自己申告の限界と人間確認の必要性の背景） | 2026-07-15 |

注：LessWrong 等のコミュニティ記事は、必要に応じて補足として参照しうるが、本学習用資料では一次資料として扱わない（今回は掲載していない）。

## 12. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | 2026-07-15 | 旧 self_justification_bias.md を簡易版・詳細版へ分割し、詳細版として新規作成。確認済みの一次資料・関連研究・補助資料を掲載（Split from former self_justification_bias.md; created as detail version with verified references） | Takashi Oikawa |
