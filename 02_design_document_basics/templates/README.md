<!-- このファイルはテンプレートです。コピーして、各項目を自分のプロジェクトの内容に書き換えて使ってください。 -->
<!-- 未確定の項目は、空欄のままか「未確定」と書き、推測を事実として書かないこと。 -->
<!-- 本テンプレートは学習用・小規模ポートフォリオ用の派生版です。ファイル名・README を含む7ファイル構成・各文書の責務は、実務正本と一致させています。 -->
<!--
実務正本（Single Source of Truth）について:
- 正本リポジトリ: solacom_main（GitHub: t-oikawa-sendai/solacom_main）
- 公開区分: Private。参照には当該リポジトリへのアクセス権が必要です（一般公開されていません）。
- 正本パス（リポジトリ内相対）: docs/standards/templates/design/README.md
  設計標準の全体ルールは docs/standards/DESIGN_DOCUMENT_STANDARD.md
- 派生基準: solacom_main にタグは未設定のため、コミット 0a02282（"Update design document README standard", 2026-06-27）時点の正本を基準に派生しています。
- 本学習用資料リポジトリには正本を複製しません。Single Source of Truth を守り、二重管理で正本が古くなることを防ぐためです。正本が更新された場合は、上記コミット以降の差分を確認して本テンプレートへ反映します。
-->
<!--
README作成方針（初学者向け）
- README は設計書群の表紙・入口とする
- 文章は最短にする。詳細は個別 Doc（01〜06）へ誘導する
- スクリーンショットは最小サイズの代表画像のみ掲載する
- 画面を持たない場合は「対象外。理由：画面を持たないため。」と書いてよい
- 個人情報・機密情報・APIキー・トークンが写る画像は使用禁止
- Change History は作業メモにしない
-->

# Design Documents Index（設計書一覧）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | （記入例: PRJ-README。PRJ を自分のプロジェクト略号に置き換える） |
| Version（バージョン） | 0.1 |
| Status（ステータス） | Draft |
| Created Date（作成日） | （作成日 YYYY-MM-DD） |
| Last Updated（最終更新日） | （最終更新日 YYYY-MM-DD） |
| Owner（管理者） | （管理者名） |
| Related Documents（関連文書） | 01_REQUEST_DEFINITION.md 〜 06_OPERATION_AND_HANDOFF.md |

---

## Table of Contents（目次）

1. [Project Overview（プロジェクト・機能の概要）](#1-project-overviewプロジェクト機能の概要)
2. [Problem / Solution / Benefit Summary（問題・解決・効果の概要）](#2-problem--solution--benefit-summary問題解決効果の概要)
3. [Screen Overview（画面概要）](#3-screen-overview画面概要)
4. [Design Documents Index（設計書一覧）](#4-design-documents-index設計書一覧)
5. [Overall Design Policy（設計上の全体方針・前提）](#5-overall-design-policy設計上の全体方針前提)
6. [Glossary（用語集・略語定義）](#6-glossary用語集略語定義)
7. [Document Owners and Reviewers（文書管理者・レビュアー一覧）](#7-document-owners-and-reviewers文書管理者レビュアー一覧)
8. [Change History（変更履歴）](#8-change-history変更履歴)

---

## 1. Project Overview（プロジェクト・機能の概要）

<!-- このプロジェクト・機能が何を目的としているかを1〜3文で記述する -->

（記入欄）

---

## 2. Problem / Solution / Benefit Summary（問題・解決・効果の概要）

<!-- 各項目は1〜2文の概要のみ。詳細は下記 Doc へ誘導する -->

| Item（項目） | Summary（概要） | Detail Document（詳細文書） |
|---|---|---|
| Current Problems（現在の問題点） | （記入欄） | [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) |
| Development Purpose（開発目的） | （記入欄） | [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) |
| Solution Approach（解決方針） | （記入欄） | [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) |
| System Functions（システム機能） | （記入欄） | [02_REQUIREMENTS_DEFINITION.md](./02_REQUIREMENTS_DEFINITION.md) |
| Expected Benefits（期待効果） | （記入欄） | [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) |
| Completion Criteria（完成判定基準） | （記入欄） | [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) |

---

## 3. Screen Overview（画面概要）

<!-- 代表画面のみ掲載する。full の詳細画像・画面項目・操作フローは 04 へ分離する -->
<!-- 画面を持たない場合の記載例: 対象外。理由：画面を持たないため。 -->

（代表画面名。画面がない場合の記載例 → 対象外。理由：画面を持たないため。）

詳細（画面一覧・項目定義・操作フロー・詳細画像）: [04_UI_AND_FLOW_DESIGN.md](./04_UI_AND_FLOW_DESIGN.md)

---

## 4. Design Documents Index（設計書一覧）

<!-- 本学習用資料の設計テンプレートは README.md + 6文書の7ファイル構成で固定する。ファイルを減らさない -->

| File（ファイル名） | Document Name（文書名） | Status（ステータス） | Version（バージョン） | Owner（担当者） |
|---|---|---|---|---|
| [01_REQUEST_DEFINITION.md](./01_REQUEST_DEFINITION.md) | Request Definition（要求定義） | Draft | 0.1 | （記入欄） |
| [02_REQUIREMENTS_DEFINITION.md](./02_REQUIREMENTS_DEFINITION.md) | Requirements Definition（要件定義） | Draft | 0.1 | （記入欄） |
| [03_DATA_AND_SECURITY_DESIGN.md](./03_DATA_AND_SECURITY_DESIGN.md) | Data and Security Design（データ・セキュリティ設計） | Draft | 0.1 | （記入欄） |
| [04_UI_AND_FLOW_DESIGN.md](./04_UI_AND_FLOW_DESIGN.md) | UI and Flow Design（UI・フロー設計） | Draft | 0.1 | （記入欄） |
| [05_ARCHITECTURE_DESIGN.md](./05_ARCHITECTURE_DESIGN.md) | Architecture Design（アーキテクチャ設計） | Draft | 0.1 | （記入欄） |
| [06_OPERATION_AND_HANDOFF.md](./06_OPERATION_AND_HANDOFF.md) | Operation and Handoff Design（運用・詳細設計引き継ぎ） | Draft | 0.1 | （記入欄） |

---

## 5. Overall Design Policy（設計上の全体方針・前提）

<!-- 設計全体を通じて共有すべき方針・制約・前提を記述する -->
<!-- 個別文書に繰り返し書く必要のある共通事項をここにまとめる -->

（記入欄）

---

## 6. Glossary（用語集・略語定義）

<!-- この設計書群で使用するプロジェクト固有の用語・略語を定義する -->
<!-- 汎用的な IT 用語は記載不要 -->

| Term / Abbreviation（用語・略語） | Definition（定義） |
|---|---|
| （記入欄） | （記入欄） |

---

## 7. Document Owners and Reviewers（文書管理者・レビュアー一覧）

| Role（役割） | Name（氏名） | Assigned Documents（担当文書） |
|---|---|---|
| Document Owner（文書管理者） | （記入欄） | All Documents（全文書） |
| Reviewer（レビュアー） | （記入欄） | （記入欄） |

---

## 8. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | （作成日 YYYY-MM-DD） | Initial draft（初版作成） | （作成者） |
