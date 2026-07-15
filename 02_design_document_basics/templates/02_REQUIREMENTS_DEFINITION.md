<!-- このファイルはテンプレートです。コピーして、各項目を自分のプロジェクトの内容に書き換えて使ってください。 -->
<!-- 未確定の項目は、空欄のままか「未確定」と書き、推測を事実として書かないこと。 -->
<!-- 本テンプレートは学習用・小規模ポートフォリオ用の派生版です。ファイル名・責務は正本と一致させています。実務版の正本は solacom_main/docs/standards/templates/design/02_REQUIREMENTS_DEFINITION.md を参照してください。 -->
<!-- ここでは要件（システムが満たすべき条件＝実現側）を扱います。要求の背景説明は 01_REQUEST_DEFINITION.md に置き、ここで重複させません。 -->

# Requirements Definition（要件定義）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | （記入例: PRJ-REQUIREMENTS。PRJ を自分のプロジェクト略号に置き換える） |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | （作成日 YYYY-MM-DD） |
| Last Updated（最終更新日） | （最終更新日 YYYY-MM-DD） |
| Owner（管理者） | （管理者名） |
| Related Documents（関連文書） | README.md / 01_REQUEST_DEFINITION.md / 03_DATA_AND_SECURITY_DESIGN.md / 04_UI_AND_FLOW_DESIGN.md / 05_ARCHITECTURE_DESIGN.md |

---

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Scope（対象範囲）](#2-scope対象範囲)
3. [Out of Scope（対象外範囲）](#3-out-of-scope対象外範囲)
4. [Assumptions（前提条件）](#4-assumptions前提条件)
5. [Definition Details（定義内容）](#5-definition-details定義内容)
6. [Open Issues（未決事項）](#6-open-issues未決事項)
7. [Handoff to Detail Design（詳細設計への引き継ぎ）](#7-handoff-to-detail-design詳細設計への引き継ぎ)

---

## 1. Purpose（目的）

<!-- この文書が何を定義し、誰に向けて書かれているかを記述する -->
<!-- 要件は、要求（何を達成したいか）を実現するために、システムが満たすべき条件を具体化するもの -->

（記入欄）

---

## 2. Scope（対象範囲）

<!-- この文書がカバーする機能・システム・フェーズを記述する -->

（記入欄）

---

## 3. Out of Scope（対象外範囲）

<!-- 明示的にスコープ外とするものを記述する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

（記入欄）

---

## 4. Assumptions（前提条件）

<!-- この文書の内容が成立するために必要な前提を記述する -->
<!-- 要求側の前提と重複させず、要件として必要な前提だけを書く -->

（記入欄）

---

## 5. Definition Details（定義内容）

### 5.1 Functional Requirements（機能要件一覧）

<!-- システムが「何をするか」を記述する。ID・優先度（High / Medium / Low）・詳細を記載する -->

| ID | Feature Name（機能名） | Priority（優先度） | Details（詳細） |
|---|---|---|---|
| FR-001 | （記入欄） | High | （記入欄） |

### 5.2 Non-Functional Requirements（非機能要件）

<!-- 性能・使いやすさ・安全性など、機能以外の品質条件を記述する -->
<!-- セキュリティ要求レベルはここに記載する -->
<!-- セキュリティの設計仕様（認証・認可・通信・保存・個人情報保護の実装方針）は 03_DATA_AND_SECURITY_DESIGN.md に記載する -->

| Type（種別） | Requirement（要件内容） |
|---|---|
| Performance（性能） | （記入欄） |
| Availability（可用性） | （記入欄） |
| Security Requirement Level（セキュリティ要求レベル） | （記入欄） |
| Maintainability（保守性） | （記入欄） |
| Other（その他） | （記入欄） |

### 5.3 Screen List（画面一覧）

<!-- 画面名・利用目的の概要まで記載する -->
<!-- 画面項目・レイアウト・操作・遷移の詳細は 04_UI_AND_FLOW_DESIGN.md に記載する -->

| Screen ID（画面ID） | Screen Name（画面名） | Purpose / Overview（利用目的・概要） |
|---|---|---|
| SCR-001 | （記入欄） | （記入欄） |

### 5.4 API Overview（API一覧の概要）

<!-- 外部公開・内部利用 API の概要を記載する -->
<!-- API 詳細仕様は 05_ARCHITECTURE_DESIGN.md に記載する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

| API ID | API Name / Endpoint Overview（API名 / エンドポイント概要） | Purpose（用途） |
|---|---|---|
| API-001 | （記入欄） | （記入欄） |

### 5.5 Data Overview（データ種別・件数規模の概要）

<!-- 扱うデータの種別・想定件数・規模感を記述する -->
<!-- 詳細なデータ設計は 03_DATA_AND_SECURITY_DESIGN.md に記載する -->

| Data Type（データ種別） | Estimated Volume（想定件数・規模） | Notes（備考） |
|---|---|---|
| （記入欄） | （記入欄） | （記入欄） |

### 5.6 Mapping to Request Definition（要求定義との対応マッピング）

<!-- 01_REQUEST_DEFINITION.md のユーザーストーリー ID と機能要件 ID を対応付ける -->
<!-- 例: US-001 → FR-001, FR-002。要求に対応しない過剰な要件がないか見直す -->

| User Story ID（ユーザーストーリー ID） | Functional Requirement ID（対応する機能要件 ID） |
|---|---|
| （記入欄） | （記入欄） |

---

## 6. Open Issues（未決事項）

| ID | Open Issue（未決事項） | Owner（担当者） | Due Date（期限） | Status（ステータス） |
|---|---|---|---|---|
| TBD-001 | （記入欄） | （記入欄） | （記入欄） | Open |

---

## 7. Handoff to Detail Design（詳細設計への引き継ぎ）

<!-- 実装フェーズに伝えるべき設計意図・判断経緯・注意事項を記述する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

（記入欄）
