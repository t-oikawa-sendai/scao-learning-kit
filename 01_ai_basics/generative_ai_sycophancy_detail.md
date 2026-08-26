# 生成AIの迎合と摩擦回避 詳細編

> **[発展]** 生成AI利用の基礎で迎合の概要を理解した後、検出・検証・運用上の対策を深掘りするための資料。

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L1-SYCO-DETAIL |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [01 一覧](./README.md) / [生成AI利用の基礎 -202608-](./generative_ai_usage_overview.md) / [生成AIの自己正当化バイアス 詳細編](./self_justification_bias_detail.md) |

---

## 1. Purpose（目的）

生成AIが利用者の主張・前提へ合わせすぎるように見える出力を、観測可能な挙動として整理し、検出・検証・対策方法を理解する。

---

## 2. 操作上の定義

本教材でいう「迎合」は、生成AIが利用者の主張・好み・前提へ過剰に適応し、必要な指摘・反論・検証を弱めるように見える出力挙動を指す。

Anthropicの研究では、RLHFで訓練された複数のAI Assistantにおいて、利用者の信念と一致する回答をTruthfulな回答より選ぶSycophancyが観測されている。[Anthropic Research](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models)

ここで扱うのは出力挙動であり、AIが感情、自尊心、対立回避の意思を持つと断定するものではない。

---

## 3. 自己正当化に見える出力との違い

| テーマ | 主に確認する対象 |
|---|---|
| 迎合 | **利用者の主張**へ合わせ、必要な反論・訂正が弱くなるように見える出力 |
| 自己正当化に見える出力 | **AI自身の過去回答**を撤回せず維持するように見える出力 |

両者は同時に起こる場合があるが、同じ問題として扱わない。

---

## 4. 観測しやすいパターン

- 利用者の主張を事実確認せず前提化する。
- 明確な問題があっても「良いと思います」と肯定から入る。
- 利用者から強く主張された後、根拠より同意を優先する。
- 「どちらも正しい」として必要な判断を避ける。
- 謝罪だけで論点を閉じ、何が誤りだったかを確定しない。

丁寧な回答であることと、正確な回答であることは別である。

---

## 5. 検出と検証

### 5.1 正本と照合する

SPEC、README、設計書、公式Documentation等と照合する。

利用者の発言と正本が食い違う場合は、その差を明示して確認する。

### 5.2 Evidenceを確認する

「利用者がそう言った」「AIが以前そう答えた」を根拠にしない。

技術的事実は一次情報へ戻って確認する。

### 5.3 独立したReviewを使う

重要な成果物は、作成したAIと同じContextだけで最終判定しない。

必要に応じて別のAI、人間、Test、Git差分等を利用する。

---

## 6. 利用者側の対策

### 6.1 反論を許可する

次のような指示は、批判的な観点を求めることを明確にするために使える。

> 迎合せずに確認してください。問題点・矛盾・抜け漏れがあれば、根拠を示して反論してください。

この一文だけで迎合を完全に防げるわけではない。正本照合やEvidence確認と組み合わせる。

### 6.2 ASKMEを使う

利用者の発言だけでは重要な判断が確定できない場合、同意して進めさせるのではなくASKMEさせる。

### 6.3 謝罪より訂正を求める

誤りがあった場合は、謝罪で終わらせず、何が誤りだったか、何を根拠に修正するかを確認する。

---

## 7. Practical Checkpoints（確認点）

- 利用者の主張を無条件に事実扱いしていないか。
- 反論すべき箇所で肯定だけになっていないか。
- 正本・一次情報との照合があるか。
- 謝罪で論点が閉じていないか。
- 同じContextだけで最終評価していないか。

---

## 8. Evidence

- **EV-007**：[Anthropic — Towards Understanding Sycophancy in Language Models](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models)

Repository全体のEvidence一覧は [EVIDENCE.md](../EVIDENCE.md) を参照する。
