# 01：AI利用の基礎

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-01-INDEX |
| Version（バージョン） | 0.7 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [トップ](../README.md) / [02：PF設計・ドキュメント](../02_design_document_basics/README.md) / [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md) / [Evidence](../EVIDENCE.md) |

---

## 1. Purpose（目的）

職業訓練校の生徒が、学習・就職活動・PF作成・ソフトウェア開発などで生成AIを利用するための基礎を理解することを目的とする。

生成AIを「何でも正しく答える道具」として扱うのではなく、どのような仕組み・特性を持ち、どこまで任せられ、どこで人間の判断・確認が必要になるかを理解する。

生成AIを利用することを前提とし、「使う / 使わない」「メリット / デメリット」という二分法を主構造にはしない。**使い方によって結果がどう変わるか**を具体的な利用場面から学ぶ。

---

## 2. Target Audience（対象読者）

中心対象は職業訓練校の生徒とする。

教材上は、初心者と中級者を代表像として扱うが、教材側がテストや用語知識で読者を分類しない。読者自身が理解度・経験・読みやすさに応じて選択する。

初心者と中級者で扱う主題は原則として共通とし、説明の深さ・用語補足・具体例の量を調整する。

---

## 3. Learning Priority（学習優先度）

この領域では、資料を次の3区分で案内する。

### 基礎

最初に理解してほしい共通内容。

1. [生成AI利用の基礎 -202608-](./generative_ai_usage_overview.md)
2. [生成AI利用時の安全ルール](./ai_safety_basic.md)
3. [生成AIへの指示方法](./how_to_instruct_generative_ai.md)

### [発展]

現時点で理解必須ではない。必要になった場合、理解を深めたい場合に読む。

- [LITM（Lost in the Middle）と文脈管理](./litm_and_context_management.md)
- [生成AIの自己正当化バイアス 詳細編](./self_justification_bias_detail.md)
- [生成AIの迎合と摩擦回避 詳細編](./generative_ai_sycophancy_detail.md)

`[発展]` は中級者専用ではない。初心者も必要に応じて参照できる。

### [補助資料]

難易度ではなく、必要な場面で利用する実践資料。

- [AI専用・新チャット文脈移行プロトコル](./migration_context_template.md)

---

## 4. Learning Flow（学習の流れ）

```text
生成AIを何に使えるか知る
        ↓
使い方によって結果が変わることを理解する
        ↓
生成AIの全体像・特性・限界を知る
        ↓
安全な利用方法を確認する
        ↓
AIへの指示方法を学ぶ
        ↓
必要に応じて [発展] / [補助資料] を参照する
```

基礎3資料を読めば、日常的な生成AI利用に必要な共通土台を得られる構成とする。

---

## 5. Main Topics（主な内容）

基礎資料では、用語暗記ではなく、生成AI全体の関係を理解することを重視する。

主に扱う内容：

- 学習・就職活動・PF作成・ソフトウェア開発での利用
- 特に意識せず使う場合と、ポイントを押さえて使う場合の違い
- LLM / SLM
- Prompt / Context / Context Window / Token
- Multimodal
- Tool Use
- RAG / MCP
- Hallucination
- LITM
- 迎合
- 自己正当化に見える出力
- ASKME
- AIに任せることと、人間が判断・確認すること
- 旧モデル・軽量モデルと2026年8月時点の高性能モデルにおける指示方法の違い

---

## 6. Evidence

技術的事実、生成AIの特性、製品仕様、利用方法に関する記述は、原則として公式Documentation、公式発表、一次研究など確認可能なEvidenceに基づく。

各教材末尾に主要Evidenceを掲載する。Repository全体の外部Evidence正本は [EVIDENCE.md](../EVIDENCE.md) を参照する。

---

## 7. Current Status（現在状態）

`01_ai_basics/` は再構成中である。

基礎説明は `生成AI利用の基礎 -202608-` へ集約し、既存のLITM・迎合・自己正当化に関する資料は、基礎との重複を整理した上で `[発展]` の深掘り資料として扱う。

Markdownの基本はAI利用基礎ではなく文書作成の補助知識として、`02_design_document_basics/` の `[補助資料]` へ移動する。

---

## 8. Related Materials（関連資料）

- [トップに戻る](../README.md)
- [02：PF設計・ドキュメント](../02_design_document_basics/README.md)
- [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md)
- [Evidence一覧](../EVIDENCE.md)
