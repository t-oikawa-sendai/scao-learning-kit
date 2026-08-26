# CURRENT

Last Updated: 2026-08-26
Status: CURRENT

## PURPOSE

`scao-learning-kit` を、主にIT初学者が生成AIを活用してポートフォリオ（PF）を設計・実装・完成させる際に利用できる学習用資料集として整備する。

Repository全体はPF作成を中心に整理する。一方、`01_ai_basics/` はPF・開発用途だけに限定せず、職業訓練校の生徒が学習・就職活動・PF作成・ソフトウェア開発などで生成AIを利用するための共通基礎を扱う。

## CURRENT GIT STATE

- Repository: `t-oikawa-sendai/scao-learning-kit`
- Base branch: `main`
- Base commit: `27a91ea494bbc489f6910de91c58774c95aae08c`
- Working branch: `docs/ai-basics-restructure-202608`
- Working branch latest commit: `c2b90a5635d3f041f6d5a24ed49cb4a024530663`
- `main` へのmerge: 未実施
- 現在はWorking branch上で文書再構成・検証を行う。

## PERMANENT OPERATION RULES

恒久的なAI作業ルールはRepositoryルートの `AGENTS.md` を正本とする。

特にASKMEについては、利用者判断がなければ安全・正確に進められないブロッカーに限定する。主要設計判断が完了し、残りが詳細設計・文書調整になった場合は、AI側からASKME終了を明示して続行する。

## CONFIRMED ACTIVE STRUCTURE

現行の学習構造は難易度Levelではなく、利用目的を中心に次の3領域とする。

1. `01_ai_basics/`：AIを理解して使う
2. `02_design_document_basics/`：PFを設計・管理する
3. `03_portfolio_creation_guide/`：AIを使ってPFを作る

`04_ai_agentic_workflow/` は物理的には維持するが、現在の初版学習導線・初版整備対象から外す。

## 01_AI_BASICS CONFIRMED DESIGN

### 1. 対象と利用場面

中心対象は職業訓練校の生徒とする。

生成AI利用をPF作成・設計・実装だけに限定しない。主な利用場面は次とする。

- 学習
- 就職活動
- PF作成
- ソフトウェア開発
- 調査・情報整理
- 文章作成・説明整理
- アイデア整理・比較検討
- フィードバック・レビュー

生成AIを利用することを前提とし、「使う / 使わない」「メリット / デメリット」を教材の主構造にはしない。

### 2. 読者区分と学習優先度

教材上の代表像は初心者 / 中級者の2区分とするが、教材側で用語知識・経験年数等による客観判定はしない。読者本人が理解度・経験・読みやすさに応じて選択する。

初心者 / 中級者で扱う主題は原則共通とし、違いは説明の深さ・用語補足・具体例の量とする。

学習優先度は人物区分と分離する。

- 表示なし：基礎・共通内容
- `[発展]`：現時点で理解必須ではない深掘り内容
- `[補助資料]`：難易度ではなく、必要な場面で利用する実践資料

`[発展]` は中級者専用ではない。

### 3. 基礎3文書

最初に読む基礎資料は次の順序で固定する。

1. `01_ai_basics/generative_ai_usage_overview.md` — 表示タイトル `生成AI利用の基礎 -202608-`
2. `01_ai_basics/ai_safety_basic.md` — 表示タイトル `生成AI利用時の安全ルール`
3. `01_ai_basics/how_to_instruct_generative_ai.md` — 表示タイトル `生成AIへの指示方法 -202608-`

年月は表示タイトルに付け、ファイル名は固定する。将来メンテナンス時は、モデル依存内容を再確認してタイトル年月を更新する。

### 4. `生成AI利用の基礎 -202608-`

入口の中心1文書とする。用語集ではなく、文章の流れの中で全体像を理解させる。

説明順は、利用から仕組みへ進む。

1. 生成AIで何ができるか
2. 学習 / 就職活動 / PF作成 / ソフトウェア開発の4場面
3. 各場面で「特に意識せず使う場合」と「ポイントを押さえて使う場合」を比較
4. どのモデルでも共通する基本
5. モデル能力によって変わる指示方法
6. 生成AIを支える主な仕組み
7. RAG / MCP
8. Hallucination / LITM / 迎合 / 自己正当化に見える出力
9. ASKME
10. AIと人間の役割

本文中で次の概念を自然に扱う。

- AI / 生成AI
- LLM / SLM
- Prompt
- Context
- Context Window
- Token
- Multimodal
- Tool Use
- RAG
- MCP
- Hallucination
- LITM
- 迎合
- 自己正当化に見える出力
- ASKME

用語暗記用の一覧は作らない。

RAG / MCPは文章説明に加えMermaid図を使用し、RAGは主に回答に使う情報を取得する考え方、MCPは外部データ・Toolと接続するProtocolとして区別する。

Hallucinationの独立詳細文書は作らない。

### 5. 高性能モデルと旧モデル・軽量モデル

常に最新・高性能モデルを使用する前提にはしない。料金、利用制限、提供状況、速度、用途等により旧モデル・軽量モデルを使う場合も通常の利用として扱う。

モデルが違っても共通する基本と、能力によって変わる部分を明確に分ける。

2026年8月時点の高性能モデルに関する説明では、GPT-5.x系、Claude Opus 5系、Gemini 3系後半以降を念頭に置き、公式一次情報をEvidenceとして使用する。

中心メッセージは次とする。

> **「何を実現したいか」は人間が決め、「どう実現するか」のプロセスはAIに考えさせ提案させる。**

目的・Context・重要な制約・成功条件を明確にしつつ、実現方法には一定の自由度を与える。これにより、利用者自身の知識・経験だけでは思いつかなかった方法や選択肢をAIが提示できる余地を作る。

ただし、提案の採用判断と重要な結果の確認は人間が行う。

今後のモデル進化によって適切な指示方法が変わる可能性を明記する。

### 6. `生成AIへの指示方法 -202608-`

入口文書が「なぜ使い方が変わるか」を扱い、本資料は「実際にどう指示するか」を扱う。

- 全モデル共通部分とモデル能力によって変わる部分を分離する。
- 旧モデル・軽量モデル / 2026年8月時点の高性能モデルの差は、差がある項目だけ表で示す。
- 現行8要素は廃止せず、毎回すべて書くテンプレートではなくチェック観点として扱う。
- 学習 / 就職活動 / PF・開発の短い具体例を載せる。
- ASKMEを「重要な未確定事項をAIに勝手に補完させない方法」として扱う。

8つのチェック観点：

1. 目的
2. 背景・前提
3. 対象範囲
4. 変更禁止範囲
5. 完了条件
6. 検証方法
7. 停止条件
8. 出力形式

### 7. `生成AI利用時の安全ルール`

一般利用を土台とし、学習・就職活動・PF・開発を対象にする。開発固有のGit・Command・破壊的操作は後半へ置く。

個人情報は一律入力禁止とはしない。

- 本当に必要な情報か確認する。
- 利用サービスのデータ取扱い・設定を公式情報で確認する。
- 不要な個人情報は削除・マスキングする。
- 第三者情報・企業秘密は権限なしに入力しない。

製品別の設定手順は本資料では扱わない。

### 8. 深掘り資料

次を `[発展]` として残す。

- `litm_and_context_management.md`
- `generative_ai_sycophancy_detail.md`
- `self_justification_bias_detail.md`

基礎文書と重複する説明は整理し、単独で読める最小限の定義を残した上で、検出・検証・対策・運用などの深掘りに集中する。

基礎編2文書は入口文書へ吸収後、参照関係を確認した上で削除する。

- `generative_ai_sycophancy_basic.md`
- `self_justification_bias_basic.md`

### 9. 補助資料

`migration_context_template.md` は `[補助資料]` とし、表示タイトルを `AI専用・新チャット文脈移行プロトコル -202608-` とする。

2026年8月時点では、高性能モデル用 / 旧モデル用にテンプレートを2種類へ分割しない。引き継ぐ情報は共通であり、モデルによって調整するのは指示の細かさ・AIへ任せる範囲とする。判断根拠にはOpenAI / Google / Anthropicの公式一次情報を付ける。

### 10. Markdown

`markdown_basic.md` はAI利用基礎から外し、`02_design_document_basics/markdown_basic.md` へ移動する。

02では `[補助資料]` とし、設計そのものの必須教材にはしない。文書冒頭と02 READMEの両方で位置づけを表示する。

## EVIDENCE POLICY

技術的事実、生成AIの特性、製品仕様、利用方法に関する記述は、原則として公式Documentation、公式発表、一次研究など確認可能なEvidenceに基づく。

### Repository表示

Top README先頭に次を表示する。

- `Evidence Last Verified: YYYY-MM-DD`
- 日付表示自体を `/EVIDENCE.md` へのLinkにする。
- Evidence方針の一文をREADME上部に表示する。

`EVIDENCE.md` 冒頭にもRepository全体の `Evidence Last Verified` を表示する。

確認日はEvidence単位では持たない。

### `EVIDENCE.md`

Repositoryルート `/EVIDENCE.md` を外部Evidenceの正本とする。

各Evidenceは固定ID `EV-xxx` を持ち、IDを振り直さず、廃止番号を再利用しない。

1件の基本項目は次の5つとする。

1. Type
2. Status
3. Provider
4. Source Title
5. URL

`SUPERSEDED` の場合だけ `Replaced By` を追加する。

Type：

- `OFFICIAL_DOC`
- `OFFICIAL_ANNOUNCEMENT`
- `OFFICIAL_SPEC`
- `OFFICIAL_REPOSITORY`
- `PEER_REVIEWED`
- `PREPRINT`
- `TECHNICAL_REPORT`

Status：

- `ACTIVE`
- `SUPERSEDED`
- `RETIRED`

査読済み一次研究を優先するが、AI分野では未査読の一次研究も利用可能とし、`PREPRINT` 等で明示する。

AIベンダー公式情報について、製品仕様・公式推奨方法と、ベンダー自身による性能評価を同一視しない。必要に応じて原論文・第三者評価を併用する。

情報源に固定の優先順位は設けず、主張に対して最適な一次情報を選ぶ。二次情報だけで技術的事実を確定しない。

一次情報で確認できない内容は原則として技術的事実として教材へ載せない。必要な場合はSCAO独自の整理・仮説としてFactと分離する。

各教材では、1文ごとではなく、根拠が必要な説明単位ごとに本文中の短い一次情報Linkを置く。文書末尾にはEvidence ID + 資料名 + Linkを掲載する。

SCAO独自の教材設計判断は `EVIDENCE.md` に混在させず、本 `CURRENT.md` 等のRepository内正本で管理する。

Evidenceの自動監視・定期実行の頻度・記録単位・自動更新範囲は現在未決であり、今回の01再構成のブロッカーにはしない。

## FIXED DESIGN DOCUMENT RULES

`02_design_document_basics/templates/` の設計テンプレートは次の7ファイル構成を固定する。

- `README.md`
- `01_REQUEST_DEFINITION.md`
- `02_REQUIREMENTS_DEFINITION.md`
- `03_DATA_AND_SECURITY_DESIGN.md`
- `04_UI_AND_FLOW_DESIGN.md`
- `05_ARCHITECTURE_DESIGN.md`
- `06_OPERATION_AND_HANDOFF.md`

今回の01再構成で、この7ファイル構成・ファイル名・内容を無断変更しない。

## 03_PORTFOLIO_CREATION_GUIDE

`03_portfolio_creation_guide/` は01・02を実際のPF作成工程へつなぐ役割とする。01・02の説明を重複して大量作成せず、「いつ、どの資料を使うか」を案内する。

現在の基本フロー：

1. テーマ・目的
2. 要求
3. 要件
4. 設計書
5. AIへの実装指示
6. AI支援による実装
7. テスト
8. レビュー
9. 設計と実装の整合
10. README・GitHub・公開・提出
11. PF完成

03の詳細教材大量作成は01・02の棚卸し完了後とする。

## COMPLETED ON WORKING BRANCH

2026-08-26時点で、Working branch上では次を実施済み。

- `AGENTS.md` 新規作成。ASKME制御・Evidence・文書変更の恒久ルールを記録。
- `EVIDENCE.md` 新規作成。
- `generative_ai_usage_overview.md` 新規作成。
- ルートREADMEをEvidence Based方針と新しい01導線へ更新。
- `01_ai_basics/README.md` を基礎 / `[発展]` / `[補助資料]` へ再構成。
- `how_to_instruct_generative_ai.md` を202608時点のモデル差を踏まえて再構成。
- `ai_safety_basic.md` を一般利用・就職活動を含む安全ルールへ再構成。
- Markdownを01から02へ移動し `[補助資料]` 化。
- LITM / 迎合詳細 / 自己正当化詳細を `[発展]` として再構成。
- 迎合基礎編 / 自己正当化基礎編を入口文書へ吸収して削除。
- 文脈移行プロトコルを `-202608-` 表示とし、モデル差の一次情報Evidenceを追加。
- 04のREADMEから削除済み基礎編への参照を除去。

## CURRENT WORK

Working branchの内容について、次を検証・整合する。

- `CHANGELOG.md` 更新
- 本 `CURRENT.md` 更新
- 削除・移動したFileへの残存Link確認
- README / 01 / 02 / 04の導線整合
- Evidence ID / URL / Type / Statusの整合
- Mermaid構文確認
- 旧「メリット / デメリット」主構造の残存確認
- L1等の旧表示・旧導線の残存確認
- 7ファイル設計テンプレートが無変更であることの確認
- `main`との差分確認

## DO NOT DO YET

- Working branchを `main` へmergeしない。
- `04_ai_agentic_workflow/` を物理削除しない。
- 7ファイル設計テンプレートを変更しない。
- 03の詳細教材を大量作成しない。
- Evidence自動監視の頻度・自動更新範囲を勝手に決めない。
- 一次情報未確認のモデル仕様を教材Factとして追加しない。

## NEXT ACTION

1. `CHANGELOG.md` に2026-08-26の主要変更を反映する。
2. Working branch全体のLink・Evidence・用語・構造を検証する。
3. `main` との差分と設計テンプレート無変更を確認する。
4. 問題があればWorking branch上で修正する。
5. 検証結果を提示し、`main` 反映判断が必要になった時点でのみ停止する。

## RESUME ORDER

作業再開時は次の順で確認する。

1. `AGENTS.md`
2. `project-notes/CURRENT.md`
3. ルート `README.md`
4. 作業対象DirectoryのREADME
5. 対象資料本文
6. 必要時のみ `CHANGELOG.md`
