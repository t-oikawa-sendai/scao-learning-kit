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
| 0.1 | 2026-07-15 | `01_ai_basics/generative_ai_sycophancy_basic.md` | Added | 初版作成。生成AIの迎合と摩擦回避を出力挙動として整理。典型兆候・外部ブレーキ・合言葉「# 迎合なし　反論歓迎」の都度再投入運用・AIを御する4つの心得概要を記載 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `01_ai_basics/generative_ai_sycophancy_detail.md` | Added | 初版作成。sycophancy関係・AIを御する4つの心得・合言葉運用・ルール実体化・4AI役割分離を詳細化。自己正当化バイアスとの責務分離を明記 | Takashi Oikawa |
| 0.1 | 2026-07-15 | `04_ai_agentic_workflow/claude_code_reference.md` | Added | 初版作成。Claude Codeの概念参考資料。チャットとの違い・調査計画編集検証・権限・SCAO役割境界を整理。変動する具体手順は推測せず公式確認を明記 | Takashi Oikawa |
| 0.6 | 2026-07-15 | `01_ai_basics/README.md` | Changed | 迎合と摩擦回避の基礎編・詳細編への導線を追加。学習用資料数を9点へ更新 | Takashi Oikawa |
| 0.6 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Changed | Claude Code参考資料への導線を追加。Usage Guide・現在状態を部分公開に合わせて更新 | Takashi Oikawa |
| 0.8 | 2026-07-15 | `README.md` | Changed | L1索引へ迎合・摩擦回避を追加。L4へClaude Code参考資料を追加。目的別導線・用語集・構成概要を更新 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `01_ai_basics/self_justification_bias_basic.md` | Changed | 生成AIの出力挙動中心へ再設計。タイトルを「生成AIの自己正当化バイアス 基礎編」へ変更。人間心理学中心の章を削除し名称由来へ縮小。誤り対応4ステップ・停止条件・SCAOの4AI役割分離を明記。ファイル名は未変更 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `01_ai_basics/self_justification_bias_detail.md` | Changed | 生成AIの出力挙動中心へ再設計。タイトルを「生成AIの自己正当化バイアス 詳細編」へ変更。人間心理学中心の章を名称由来へ縮小。出力パターン・自己評価・自己訂正・正本照合・sycophancy・4AI役割分離を整理。ファイル名は未変更 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `01_ai_basics/README.md` | Changed | 対象2文書の表示名・説明を出力挙動中心のタイトルへ統一 | Takashi Oikawa |
| 0.7 | 2026-07-15 | `README.md` | Changed | L1索引の表示名と用語集の自己正当化バイアス定義を出力挙動中心へ更新 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `01_ai_basics/how_to_instruct_generative_ai.md` | Changed | 自己正当化バイアス基礎へのリンク表示名を「基礎編」へ整合 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Changed | 詳細編への参照タイトルと対象読者の表現を新タイトルへ整合 | Takashi Oikawa |
| 0.6 | 2026-07-15 | `README.md` | Changed | 生成AI関連用語を統一。学習用資料一覧・導線・用語集を更新。基本用語を生成AIとし、AI／LLM／AIエージェントの使用範囲と指示／プロンプトの責務を整理。口語「AIへの頼み方」等を除去 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `01_ai_basics/how_to_instruct_generative_ai.md` | Changed | `how_to_ask_ai.md` を rename。タイトルを「生成AIへの指示方法」へ変更。指示とプロンプトの関係を明記し、口語表現を整理 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `01_ai_basics/README.md` | Changed | 入口タイトル・目的・資料一覧・利用方法を生成AI用語体系へ整合。rename後の指示方法文書へのリンクを更新 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/ai_safety_basic.md` | Changed | タイトルを「生成AI利用時の安全ルール」へ変更。本文のサービス総称を生成AIへ、ツール利用主体をAIエージェントへ整理 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/litm_and_context_management.md` | Changed | 文脈参照の限界をLLM、対話主体を生成AIとして用語整理。指示方法文書へのリンクを更新 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/markdown_basic.md` | Changed | 生成AIへの構造化指示の説明へ用語整理。指示方法文書へのリンクを更新 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `01_ai_basics/self_justification_bias_basic.md` | Changed | 主題は維持し、サービス総称を生成AIへ用語整理。関連リンクを新ファイル名・新タイトルへ更新 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `01_ai_basics/self_justification_bias_detail.md` | Changed | 主題は維持し、類似出力挙動は生成AI、自己訂正限界はLLMとして用語整理。4AI・禁止表現・参考URLは維持 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `02_design_document_basics/README.md` | Changed | L1参照名と実装前の「指示」表現を生成AI用語体系へ整合 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `02_design_document_basics/simple_design_basic.md` | Changed | 「AIに頼む」等の口語を除去し、生成AIへの実装指示表現へ統一 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `02_design_document_basics/document_management_basic.md` | Changed | 生成AIへの指示表現と安全ルール文書名を用語体系へ整合。CHANGELOGへの相対リンク切れを修正 | Takashi Oikawa |
| 0.4 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Changed | L1参照名・自己正当化詳細タイトル・同じ生成AI独占禁止の表現を用語体系へ整合 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/migration_context_template.md` | Changed | 関連リンクを指示方法文書へ更新。「今回の最初の依頼」を「今回の最初の指示」へ用語整理 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/06_OPERATION_AND_HANDOFF.md` | Changed | コメント内の実装依頼表現を生成AIへの実装指示へ用語整理 | Takashi Oikawa |
| 0.2 | 2026-07-15 | `02_design_document_basics/templates/README.md` | Fixed | CHANGELOGへの相対リンク切れを修正（`../../../` → `../../`） | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/self_justification_bias_basic.md` | Fixed | 誤テーマ Self-Attribution Bias を訂正し、Self-Justification Bias（自己正当化バイアス）を主題として概念・事例・参考資料を全面再構成。ファイル名を `self_attribution_bias_basic.md` から rename | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/self_justification_bias_detail.md` | Fixed | 誤テーマ Self-Attribution Bias／自己監視の限界を訂正し、自己正当化に類似した出力挙動と自己訂正の限界へ全面再構成。人間の心理現象とAI出力挙動を分離。ファイル名を `self_attribution_bias_detail.md` から rename | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/README.md` | Changed | 学習用資料一覧・目的文を自己正当化バイアスへ更新し、基礎／詳細へのリンクを新ファイル名へ修正 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `01_ai_basics/how_to_ask_ai.md` | Changed | 関連リンクと迎合対策の参照先を自己正当化バイアス基礎へ更新 | Takashi Oikawa |
| 0.5 | 2026-07-15 | `README.md` | Changed | L1索引・学習機能説明・用語集を自己正当化バイアスへ更新。旧ファイル名リンクを新ファイル名へ修正 | Takashi Oikawa |
| 0.3 | 2026-07-15 | `04_ai_agentic_workflow/README.md` | Changed | 対象読者・Usage Guide の参照を自己正当化バイアス詳細へ更新 | Takashi Oikawa |
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
