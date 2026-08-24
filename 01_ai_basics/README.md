# 01：AI利用の基礎

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-01-INDEX |
| Version（バージョン） | 0.7 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-24 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [トップ](../README.md) / [02：PF設計・ドキュメント](../02_design_document_basics/README.md) / [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md) |

---

## 1. Purpose（目的）

PF作成で生成AIを利用する前に、生成AIの基本的な使い方、便利な点、限界、利用時の注意事項を理解することを目的とする。

生成AIを「何でも正しく答える道具」として扱うのではなく、得意なことと苦手なことを理解し、人間が確認・判断しながら利用できる状態を目指す。

---

## 2. Target Audience（対象読者）

- 生成AIを使い始めたIT初学者
- 生成AIを使ってPFや小規模アプリを作りたい人
- 生成AIを使っているが、指示方法や回答の確認方法がまだ定まっていない人

---

## 3. Learning Structure（学習構造）

この領域では、内容を次の3つに分けて理解する。

### A. 生成AIの使い方

- [Markdownの基本](./markdown_basic.md)
- [生成AIへの指示方法](./how_to_instruct_generative_ai.md)

生成AIへ目的・条件・前提・出力形式などを伝えるための基礎を扱う。

### B. 生成AIの限界・注意事項

- [生成AI利用時の安全ルール](./ai_safety_basic.md)
- [LITM（Lost in the Middle）と文脈管理](./litm_and_context_management.md)
- [生成AIの自己正当化バイアス 基礎編](./self_justification_bias_basic.md)
- [生成AIの自己正当化バイアス 詳細編](./self_justification_bias_detail.md)
- [生成AIの迎合と摩擦回避 基礎編](./generative_ai_sycophancy_basic.md)
- [生成AIの迎合と摩擦回避 詳細編](./generative_ai_sycophancy_detail.md)
- [移行テンプレート](./migration_context_template.md)

回答の誤り、長い文脈での情報参照、迎合、秘密情報、チャット継続時の文脈管理など、生成AI利用時に注意すべき事項を扱う。

### C. 生成AIのメリット・デメリット

PF作成時に「何を生成AIへ任せると有効か」「どのような場面では人間の判断が必要か」を初心者向けにまとめる資料は、現在不足している。

この領域は今後の追加対象とする。

---

## 4. Current Materials（現在の学習用資料）

| Category（分類） | Material（資料） | Status（状態） |
|---|---|---|
| 利用方法 | Markdownの基本 | Draft |
| 利用方法 | 生成AIへの指示方法 | Draft |
| 注意事項 | 生成AI利用時の安全ルール | Draft |
| 注意事項 | LITMと文脈管理 | Draft |
| 注意事項 | 生成AIの自己正当化バイアス 基礎編 | Draft |
| 注意事項 | 生成AIの自己正当化バイアス 詳細編 | Draft |
| 注意事項 | 生成AIの迎合と摩擦回避 基礎編 | Draft |
| 注意事項 | 生成AIの迎合と摩擦回避 詳細編 | Draft |
| 文脈管理 | 移行テンプレート | Draft |
| メリット・デメリット | 専用資料 | 未作成 |

---

## 5. Usage Guide（利用方法）

PF作成前に、少なくとも次の内容を確認することを推奨する。

1. 生成AIへの指示方法
2. 生成AI利用時の安全ルール
3. 生成AIの回答をそのまま正しいと扱わないための注意事項

Markdown、LITM、迎合、自己正当化に類似した出力挙動、移行テンプレートは、必要になった時点で参照してよい。

---

## 6. Current Status（現在状態）

既存の9資料は利用可能なDraftとして維持する。

ただし、上位構造をPF作成中心へ整理した結果、「生成AIのメリット・デメリット・限界を初心者向けに俯瞰する資料」が不足していることを明示する。

既存資料の削除・統合はまだ行わず、内容重複と役割を確認した上で判断する。

---

## 7. Related Materials（関連資料）

- [トップに戻る](../README.md)
- [02：PF設計・ドキュメント](../02_design_document_basics/README.md)
- [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md)
