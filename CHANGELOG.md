# CHANGELOG

## Purpose（目的）

本ファイルは、SCAO Learning Kit リポジトリおよび配下 Markdown 文書の変更履歴を一元管理する。
各 Markdown 文書内の Change History 章は使用せず、Document Information の現在値と本 CHANGELOG を参照する。

## What to Record（記録対象）

利用者・開発者・運用担当者・レビュー担当者の判断に影響する重要変更を記録する。
意味・仕様・運用・構成に影響しない軽微な変更（明白な誤字、空白調整など）は原則記録不要。

## Category Definitions（変更分類）

| Category | 日本語 | 用途 |
|---|---|---|
| Added | 追加 | 新しい機能、章、文書、運用項目 |
| Changed | 変更 | 既存仕様、構成、手順の変更 |
| Fixed | 修正 | 誤り、不整合、不具合の修正 |
| Removed | 削除 | 機能、記述、文書の廃止 |
| Security | セキュリティ | セキュリティまたは個人情報保護上の変更 |

Git 履歴は差分確認の補助として利用する。CHANGELOG の代替とはしない。

## Change History（変更履歴）

新しい履歴を上、古い履歴を下に記載する。

| Version | Date | Document | Category | Changes | Author |
|---|---|---|---|---|---|
| 0.3 | 2026-07-15 | `02_design_document_basics/README.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `02_design_document_basics/document_management_basic.md` | Changed | 履歴管理方式を README＋CHANGELOG の2者方式へ変更。各 Markdown 文書内 Change History の併存規定を廃止（4.3・4.4 等を改訂） | Takashi Oikawa |
| 0.3 | 2026-07-15 | `02_design_document_basics/readme_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `02_design_document_basics/request_definition_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `02_design_document_basics/requirements_definition_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `02_design_document_basics/simple_design_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `README.md` | Changed | Change History 章を削除し CHANGELOG.md へのリンクを追加。履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/README.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/ai_safety_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/how_to_ask_ai.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/litm_and_context_management.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/markdown_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/migration_context_template.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/self_attribution_bias_basic.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `01_ai_basics/self_attribution_bias_detail.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/01_REQUEST_DEFINITION.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/02_REQUIREMENTS_DEFINITION.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/03_DATA_AND_SECURITY_DESIGN.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/04_UI_AND_FLOW_DESIGN.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/05_ARCHITECTURE_DESIGN.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/06_OPERATION_AND_HANDOFF.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/README.md` | Changed | Change History 章を削除し CHANGELOG.md へのリンクを追加。履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `03_portfolio_creation_guide/README.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Changed | Change History 章を削除し、履歴管理をリポジトリルート CHANGELOG.md へ移行 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `README.md` | Changed | 対象読者をIT職業訓練校に限定しない初学者一般（受講生・独学者・ポートフォリオ作成者などを含む）へ整理し、Project Overview と全体方針を整合。文書内の「教材」表現を「学習用資料」へ用語統一 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `README.md` | Changed | L2設計テンプレートを独自4ファイル構成から正本準拠の7ファイル構成（README.md + 6文書）へ修正。教材一覧・教材機能・解決方針・用語集を7ファイル構成へ整合、旧テンプレート名リンクを更新 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `README.md` | Added | 初版作成（L1・L2 初版、L3・L4 準備中）。設計標準READMEの管理形式を継承した教材向け派生READMEへ整備（Initial draft; restructured into learning-oriented derived README） | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/document_management_basic.md` | Changed | 版番号（Version）の運用基準を明文化（4.3 を追加、以降の節を繰り下げ） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/document_management_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.3 | 2026-07-15 | `02_design_document_basics/simple_design_basic.md` | Changed | 簡易設計の定義（文書数ではなく詳細度を絞ること）と、標準7ファイル構成における設計文書03〜06の責務・記載可否を明確化。リンクの不要な半角空白を修正 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/simple_design_basic.md` | Changed | 標準7ファイル構成を前提とする説明へ修正（4設計書を簡易統合した派生版という記述を削除し、各内容を標準設計ドキュメント03〜06への対応表へ置換）。旧テンプレートへのリンクを設計テンプレート一覧へ更新 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/simple_design_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/README.md` | Changed | 設計テンプレートを独自4ファイル構成から正本準拠の7ファイル構成（README.md + 6文書）へ修正。テンプレート一覧・現在状態・ファイル名統一の目的を反映 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/README.md` | Added | Initial draft（初版作成）。管理形式準拠のLevel入口READMEへ整備 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/requirements_definition_basic.md` | Changed | 設計テンプレートの7ファイル構成化に伴い、テンプレートへのリンクを 02_REQUIREMENTS_DEFINITION.md へ更新し、引き継ぎ項目の説明を正本の章名（詳細設計への引き継ぎ）へ整合 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/requirements_definition_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/request_definition_basic.md` | Changed | 設計テンプレートの7ファイル構成化に伴い、テンプレートへのリンクを 01_REQUEST_DEFINITION.md へ更新し、引き継ぎ項目の説明を正本の章名（詳細設計への引き継ぎ）へ整合 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/request_definition_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/readme_basic.md` | Changed | 設計テンプレートの7ファイル構成化に伴い、テンプレートへのリンクを README.md（設計書一覧テンプレート）へ更新 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `02_design_document_basics/readme_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/self_attribution_bias_detail.md` | Changed | 旧 self_justification_bias.md を簡易版・詳細版へ分割し、詳細版として新規作成。確認済みの一次資料・関連研究・補助資料を掲載（Split from former self_justification_bias.md; created as detail version with verified references） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/self_attribution_bias_basic.md` | Changed | 旧 self_justification_bias.md を簡易版・詳細版へ分割し、簡易版として新規作成（Split from former self_justification_bias.md; created as basic version） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/migration_context_template.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/litm_and_context_management.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/ai_safety_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/how_to_ask_ai.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/markdown_basic.md` | Added | Initial draft（初版作成） | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/README.md` | Added | Initial draft（初版作成）。管理形式準拠のLevel入口READMEへ整備 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `03_portfolio_creation_guide/README.md` | Added | Initial draft（初版作成）。準備中のまま管理形式準拠のLevel入口READMEへ整備 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Added | Initial draft（初版作成）。準備中のまま管理形式準拠のLevel入口READMEへ整備 | Takashi Oikawa |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/README.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/01_REQUEST_DEFINITION.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/02_REQUIREMENTS_DEFINITION.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/03_DATA_AND_SECURITY_DESIGN.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/04_UI_AND_FLOW_DESIGN.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/05_ARCHITECTURE_DESIGN.md` | Added | Initial draft（初版作成） | （作成者） |
| 0.1 | （作成日 YYYY-MM-DD） | `02_design_document_basics/templates/06_OPERATION_AND_HANDOFF.md` | Added | Initial draft（初版作成） | （作成者） |
