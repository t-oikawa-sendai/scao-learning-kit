# SCAO Learning Kit（学習用資料集）

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-ROOT-INDEX |
| Version（バージョン） | 0.7 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L1：生成AI利用の基本](./01_ai_basics/README.md) / [L2：設計ドキュメントの基本](./02_design_document_basics/README.md) / [L3：ポートフォリオ作成ガイド](./03_portfolio_creation_guide/README.md) / [L4：AIエージェント活用](./04_ai_agentic_workflow/README.md) / [CHANGELOG.md](./CHANGELOG.md) |

> 詳細な変更履歴は [CHANGELOG.md](./CHANGELOG.md) を参照。

> 本READMEは設計書群ではなく学習用資料集の入口であるため、solacom_main の設計標準README（`docs/standards/templates/design/README.md`）の管理形式を継承しつつ、画面概要（Screen Overview）・設計書一覧（Design Documents Index）を、学習用資料構成概要（Learning Materials Overview）・学習用資料一覧（Learning Materials Index）へ置換している。

---

## Table of Contents（目次）

1. [Project Overview（プロジェクト・学習用資料概要）](#1-project-overviewプロジェクト学習用資料概要)
2. [Problem / Solution / Benefit Summary（課題・解決・効果の概要）](#2-problem--solution--benefit-summary課題解決効果の概要)
3. [Learning Materials Overview（学習用資料構成概要）](#3-learning-materials-overview学習用資料構成概要)
4. [Learning Materials Index（学習用資料一覧）](#4-learning-materials-index学習用資料一覧)
5. [Overall Learning Policy（学習用資料全体方針）](#5-overall-learning-policy学習用資料全体方針)
6. [Glossary（用語集）](#6-glossary用語集)
7. [Document Owners and Reviewers（管理者・レビュアー）](#7-document-owners-and-reviewers管理者レビュアー)

---

## 1. Project Overview（プロジェクト・学習用資料概要）

SCAO Learning Kit は、初学者が、AIを活用してポートフォリオや小規模アプリを作成する際に、目的・要求・要件・設計・生成AIへの指示内容を整理するための学習用資料テンプレート集である。

本リポジトリは企業の本番開発手順を完全再現するものではないが、実務で重要となる設計・データ・セキュリティ・エラー処理・レビューの考え方を、ポートフォリオ作成に必要な範囲で取り入れる。必ずL1から順に読む「教科書」ではなく、目的別に参照する「学習用資料集」である。

---

## 2. Problem / Solution / Benefit Summary（課題・解決・効果の概要）

各項目は概要のみを1〜2文で示す。詳細は各Level・各学習用資料本文で扱う。

| Item（項目） | Summary（概要） | Detail Materials（詳細学習用資料） |
|---|---|---|
| Current Problems（現在の課題） | 初学者は生成AIへの指示が曖昧になりがちで、要求・要件・設計を整理しないまま作り始め、目的とずれた成果物になりやすい。 | [L1](./01_ai_basics/README.md) / [L2](./02_design_document_basics/README.md) |
| Development Purpose（開発目的） | AI活用とドキュメント整理の基礎を、初学者が短時間で身につけられる学習用資料を提供する。 | [L1](./01_ai_basics/README.md) / [L2](./02_design_document_basics/README.md) |
| Solution Approach（解決方針） | 生成AIへの指示方法・安全・文脈管理（L1）と、要求・要件・簡易設計・ドキュメント管理（L2）を、解説とコピー可能なテンプレートで学べるようにする。 | [L2 テンプレート](./02_design_document_basics/templates/README.md) |
| Learning Functions（学習用資料機能） | 解説用の学習用資料・移行テンプレート・設計ドキュメント標準の7ファイル構成テンプレート・自己正当化バイアス（基礎／詳細）を、Level別に提供する。 | [L1](./01_ai_basics/README.md) / [L2](./02_design_document_basics/README.md) |
| Expected Benefits（期待効果） | 生成AIとの意思疎通が正確になり、ポートフォリオの設計・説明の質が上がり、独立した確認（別の生成AI・人間・テスト）の習慣が身につく。 | [L1](./01_ai_basics/README.md) |
| Completion Criteria（完了判定基準） | L1・L2の考え方を土台に、要求→要件→簡易設計を自力で整理し、生成AIへ具体的な実装指示ができる状態になること。 | [L2](./02_design_document_basics/README.md) |

---

## 3. Learning Materials Overview（学習用資料構成概要）

本学習用資料集は、Level（L1〜L4）で構成する。L1・L2は初版として利用可能、L3・L4は準備中である。

- L1：生成AIを安全かつ正確に使うための基本（指示方法・Markdown・安全・LITM・自己正当化バイアス・移行テンプレート）。
- L2：作る前に整理すべき設計ドキュメントの基本（README・要求・要件・簡易設計・ドキュメント管理）と、コピーして使える設計ドキュメント標準の7ファイル構成テンプレート（README.md + 6文書）。
- L3：ポートフォリオを設計から公開・提出まで仕上げる手順（準備中）。
- L4：人間確認を挟みながらAIエージェントを活用する方法（準備中）。

読みたい項目から参照してよいが、生成AIで成果物を作る場合はL1・L2の考え方を土台として確認することを推奨する。

---

## 4. Learning Materials Index（学習用資料一覧）

| Level | Material（学習用資料） | Status（状態） | Link（リンク） |
|---|---|---|---|
| L1 | 生成AI利用の基本（入口） | Draft（利用可能） | [01_ai_basics/README.md](./01_ai_basics/README.md) |
| L1 | Markdownの基本 | Draft | [markdown_basic.md](./01_ai_basics/markdown_basic.md) |
| L1 | 生成AIへの指示方法 | Draft | [how_to_instruct_generative_ai.md](./01_ai_basics/how_to_instruct_generative_ai.md) |
| L1 | 生成AI利用時の安全ルール | Draft | [ai_safety_basic.md](./01_ai_basics/ai_safety_basic.md) |
| L1 | LITMと文脈管理 | Draft | [litm_and_context_management.md](./01_ai_basics/litm_and_context_management.md) |
| L1 | 生成AIの自己正当化バイアス 基礎編 | Draft | [self_justification_bias_basic.md](./01_ai_basics/self_justification_bias_basic.md) |
| L1 | 生成AIの自己正当化バイアス 詳細編 | Draft | [self_justification_bias_detail.md](./01_ai_basics/self_justification_bias_detail.md) |
| L1 | 移行テンプレート | Draft | [migration_context_template.md](./01_ai_basics/migration_context_template.md) |
| L2 | 設計ドキュメントの基本（入口） | Draft（利用可能） | [02_design_document_basics/README.md](./02_design_document_basics/README.md) |
| L2 | READMEの基本 | Draft | [readme_basic.md](./02_design_document_basics/readme_basic.md) |
| L2 | 要求の基本 | Draft | [request_definition_basic.md](./02_design_document_basics/request_definition_basic.md) |
| L2 | 要件の基本 | Draft | [requirements_definition_basic.md](./02_design_document_basics/requirements_definition_basic.md) |
| L2 | 簡易設計の基本 | Draft | [simple_design_basic.md](./02_design_document_basics/simple_design_basic.md) |
| L2 | ドキュメント管理の基本 | Draft | [document_management_basic.md](./02_design_document_basics/document_management_basic.md) |
| L2 | 設計テンプレート: README.md（設計書一覧） | Draft | [templates/README.md](./02_design_document_basics/templates/README.md) |
| L2 | 設計テンプレート: 01_REQUEST_DEFINITION.md（要求定義） | Draft | [templates/01_REQUEST_DEFINITION.md](./02_design_document_basics/templates/01_REQUEST_DEFINITION.md) |
| L2 | 設計テンプレート: 02_REQUIREMENTS_DEFINITION.md（要件定義） | Draft | [templates/02_REQUIREMENTS_DEFINITION.md](./02_design_document_basics/templates/02_REQUIREMENTS_DEFINITION.md) |
| L2 | 設計テンプレート: 03_DATA_AND_SECURITY_DESIGN.md（データ・セキュリティ設計） | Draft | [templates/03_DATA_AND_SECURITY_DESIGN.md](./02_design_document_basics/templates/03_DATA_AND_SECURITY_DESIGN.md) |
| L2 | 設計テンプレート: 04_UI_AND_FLOW_DESIGN.md（UI・フロー設計） | Draft | [templates/04_UI_AND_FLOW_DESIGN.md](./02_design_document_basics/templates/04_UI_AND_FLOW_DESIGN.md) |
| L2 | 設計テンプレート: 05_ARCHITECTURE_DESIGN.md（アーキテクチャ設計） | Draft | [templates/05_ARCHITECTURE_DESIGN.md](./02_design_document_basics/templates/05_ARCHITECTURE_DESIGN.md) |
| L2 | 設計テンプレート: 06_OPERATION_AND_HANDOFF.md（運用・詳細設計引き継ぎ） | Draft | [templates/06_OPERATION_AND_HANDOFF.md](./02_design_document_basics/templates/06_OPERATION_AND_HANDOFF.md) |
| L3 | ポートフォリオ作成ガイド | 準備中 | [03_portfolio_creation_guide/README.md](./03_portfolio_creation_guide/README.md) |
| L4 | AIエージェント活用 | 準備中 | [04_ai_agentic_workflow/README.md](./04_ai_agentic_workflow/README.md) |

### 目的から選ぶ導線

- 生成AIへの指示方法や安全な使い方を知りたい → [L1：生成AI利用の基本](./01_ai_basics/README.md)
- 作る前に要求・要件・設計を整理したい → [L2：設計ドキュメントの基本](./02_design_document_basics/README.md)
- ポートフォリオの作り方の全体像を知りたい → [L3：ポートフォリオ作成ガイド（準備中）](./03_portfolio_creation_guide/README.md)
- AIエージェントの活用を知りたい → [L4：AIエージェント活用（準備中）](./04_ai_agentic_workflow/README.md)

---

## 5. Overall Learning Policy（学習用資料全体方針）

- 本リポジトリは実務開発フレームワークそのものではなく、実務寄りの考え方を取り入れた学習用資料集である。
- SCAO 本体（設計標準・フレームワーク群）とは別物であり、その導入を前提としない。SCAO 本体の考え方の一部を初学者向けに噛み砕いて取り入れているが、標準の全構造をそのまま適用するものではない。
- 対象読者は、IT職業訓練校の受講生、独学者、ポートフォリオ作成やAI活用を学ぶ人など、開発や設計を学び始めた初学者一般とする。特定の教育機関専用ではない。
- 秘密情報の取り扱い注意：学習用資料の例やテンプレートに、実在するAPIキー・パスワード・トークン・秘密鍵・個人情報を記載しない。例示が必要な場合は `YOUR_API_KEY` のように、明らかにダミーと分かる文字列を使う。

---

## 6. Glossary（用語集）

| Term（用語） | Definition（定義） |
|---|---|
| SCAO | 設計標準・フレームワーク群からなる本体。本学習用資料集はその考え方の一部を学習用に噛み砕いたもので、本体とは別物。 |
| 生成AI | ChatGPT、Gemini、Claude、Cursorなど、利用者の入力に応じて文章・コード・画像等を生成するサービス・ツールの総称。 |
| LLM | 大規模言語モデル。トークン・コンテキスト・次トークン予測・推論・ハルシネーション・自己訂正など、モデル内部の特性・能力・限界を説明するときに用いる。 |
| AIエージェント | 生成AIがツール・ファイル・コマンド・外部サービスを利用し、複数工程を実行する場合の呼び方。通常の質問応答だけでは呼ばない。 |
| 指示 | 生成AIへ与える要求全体（目的・前提・対象範囲・制約・出力形式・完了条件・検証方法・停止条件など）。 |
| プロンプト | 指示を生成AIへ実際に入力する文章・質問・命令・データ。 |
| LITM（Lost in the Middle） | 長い文脈の中間にある重要情報が、相対的に参照されにくくなる傾向。 |
| 自己正当化バイアス（Self-Justification Bias） | 生成AIが過去の誤回答・誤判断・誤設計を明確に撤回せず、後付けの理由・一般論・曖昧化によって維持または補強するように見える出力挙動。心理状態の断定ではない。 |
| 要求（Request） | 何を達成したいか（目的側）の整理。 |
| 要件（Requirements） | システムが満たすべき条件（実現側）の整理。 |
| 簡易設計（Simple Design） | 要件を「どう作るか」に落とす設計の考え方。学習用・小規模向けでも設計内容は削減せず、標準の設計ドキュメント（データ・セキュリティ／UI・フロー／アーキテクチャ／運用の各文書）に分けて整理する。 |
| 正本（Canonical Document） | 「これが正しい」と定めた一次情報。重複管理を避けるための基準。 |

---

## 7. Document Owners and Reviewers（管理者・レビュアー）

| Role（役割） | Name（氏名） | Scope（担当範囲） |
|---|---|---|
| Owner（管理者） | Takashi Oikawa | 全学習用資料（All Materials） |
| Reviewer（レビュアー） | 未定（TBD） | 全学習用資料（All Materials） |
