# L1：生成AI利用の基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L1-INDEX |
| Version（バージョン） | 0.6 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [トップ](../README.md) / [L2：設計ドキュメントの基本](../02_design_document_basics/README.md) |

---

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Materials Index（学習用資料一覧）](#3-learning-materials-index学習用資料一覧)
4. [Usage Guide（利用方法）](#4-usage-guide利用方法)
5. [Current Status（現在状態）](#5-current-status現在状態)
6. [Related Materials（関連資料）](#6-related-materials関連資料)

---

## 1. Purpose（目的）

生成AIを安全に使うための基本を身につける。生成AIへの指示方法、Markdownの最小理解、秘密情報を貼らないこと、生成AI回答の確認、LITM、生成AIの自己正当化バイアス（出力挙動）、生成AIの迎合と摩擦回避（出力挙動）、チャット移行テンプレートを扱う。

## 2. Target Audience（対象読者）

- 生成AIチャットやAIエージェントを使い始めた初学者
- 生成AIを使ってポートフォリオや小規模アプリを作りたい人

## 3. Learning Materials Index（学習用資料一覧）

1. [Markdownの基本](./markdown_basic.md)
2. [生成AIへの指示方法](./how_to_instruct_generative_ai.md)
3. [生成AI利用時の安全ルール](./ai_safety_basic.md)
4. [LITM（Lost in the Middle）と文脈管理](./litm_and_context_management.md)
5. [生成AIの自己正当化バイアス 基礎編](./self_justification_bias_basic.md)
   - 生成AIが誤回答を撤回せず後付け理由で維持するように見える出力挙動を識別し、誤作業を止める。
6. [生成AIの自己正当化バイアス 詳細編](./self_justification_bias_detail.md)
   - 出力パターン、自己評価、自己訂正限界、正本照合、4AI役割分離を実務へ落とす。
7. [生成AIの迎合と摩擦回避 基礎編](./generative_ai_sycophancy_basic.md)
   - 人間の誤りや矛盾を指摘せず主張へ合わせるように見える出力挙動を識別し、外部ブレーキをかける。
8. [生成AIの迎合と摩擦回避 詳細編](./generative_ai_sycophancy_detail.md)
   - AIを御する4つの心得、合言葉運用、ルール実体化、4AI役割分離を迎合対策へ落とす。
9. [移行テンプレート](./migration_context_template.md)

## 4. Usage Guide（利用方法）

上から順に読むと理解しやすいが、必要な項目から参照してもよい。
生成AIを使って成果物を作る前に、少なくとも「生成AIへの指示方法」「生成AI利用時の安全ルール」には目を通しておくことを推奨する。

## 5. Current Status（現在状態）

初版（利用可能）。学習用資料9点すべて Draft 状態で公開している。

## 6. Related Materials（関連資料）

- [トップに戻る](../README.md)
- [L2：設計ドキュメントの基本](../02_design_document_basics/README.md)
