<!-- このファイルはテンプレートです。コピーして、各項目を自分のプロジェクトの内容に書き換えて使ってください。 -->
<!-- 未確定の項目は、空欄のままか「未確定」と書き、推測を事実として書かないこと。 -->
<!-- 本テンプレートは学習用・小規模ポートフォリオ用の派生版です。ファイル名・責務は正本と一致させています。実務版の正本は solacom_main/docs/standards/templates/design/03_DATA_AND_SECURITY_DESIGN.md を参照してください。 -->
<!-- ここではデータ（種別・保存先・個人情報）とセキュリティを扱います。画面・操作は 04、技術構成・外部連携は 05、運用・検証は 06 で扱います。 -->

# Data and Security Design（データ・セキュリティ設計）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | （記入例: PRJ-DATA。PRJ を自分のプロジェクト略号に置き換える） |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | （作成日 YYYY-MM-DD） |
| Last Updated（最終更新日） | （最終更新日 YYYY-MM-DD） |
| Owner（管理者） | （管理者名） |
| Related Documents（関連文書） | README.md / 02_REQUIREMENTS_DEFINITION.md / 05_ARCHITECTURE_DESIGN.md |

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
<!-- 扱うデータの種別・保存先・流れと、セキュリティ・個人情報の取り扱い方針を整理する -->

（記入欄）

---

## 2. Scope（対象範囲）

（記入欄）

---

## 3. Out of Scope（対象外範囲）

<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

（記入欄）

---

## 4. Assumptions（前提条件）

（記入欄）

---

## 5. Definition Details（定義内容）

### 5.1 Entity Definition and ER Diagram（エンティティ定義・ER図）

<!-- 主要なデータ（エンティティ）とその関係を記述する -->
<!-- 小規模な場合は、扱うデータ種別（例: 日付、金額、カテゴリ）の一覧でもよい -->
<!-- ER図は Mermaid / 画像 / リンクのいずれかで添付する -->

#### Entity List（エンティティ一覧）

| Entity Name（エンティティ名） | Description（説明） |
|---|---|
| （記入欄） | （記入欄） |

#### ER Diagram（ER図）

```
（ER図を記述、または画像リンクを貼る）
```

### 5.2 Table Definitions（テーブル定義）

<!-- 原則として全テーブルを記載する。一部のみ記載する場合は対象範囲と除外理由を明記する -->
<!-- データがどこから来て、どこへ保存され、どう表示されるかを意識して整理する -->
<!-- ファイル保存など DB を使わない場合: 「本文書では対象外。理由: DBを使用せず○○に保存するため」と記載する -->

#### [Table Name（テーブル名）]

| Column（カラム名） | Type（型） | NOT NULL | PK / FK | Description（説明） |
|---|---|---|---|---|
| （記入欄） | （記入欄） | （記入欄） | （記入欄） | （記入欄） |

### 5.3 Data Access and Role Design（データアクセス権限・ロール設計）

<!-- 誰がどのデータに対してどの操作を許可されるかを記述する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: 個人利用で権限区分がないため」と記載する -->

| Role Name（ロール名） | Accessible Data / Permitted Operations（アクセス可能なデータ / 操作範囲） |
|---|---|
| （記入欄） | （記入欄） |

### 5.4 Personal and Confidential Data Policy（個人情報・機密データの取り扱い方針）

<!-- 個人情報・機密データの定義・保存・アクセス制限・廃棄方針を記述する -->
<!-- 該当データがない場合: 「本文書では対象外。理由: 個人情報・機密データを扱わないため」と記載する -->

（記入欄）

### 5.5 Encryption, Masking, and Logging Policy（暗号化・マスキング・ログ取得方針）

<!-- 暗号化対象・方式、マスキング対象・方式、ログ取得対象・保存期間を記述する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

| Type（種別） | Target（対象） | Policy / Method（方式・方針） |
|---|---|---|
| Encryption（暗号化） | （記入欄） | （記入欄） |
| Masking（マスキング） | （記入欄） | （記入欄） |
| Logging（ログ取得） | （記入欄） | （記入欄） |

### 5.6 Security Design Specifications（セキュリティ設計仕様）

<!-- 認証・認可・権限・通信・保存・廃棄・個人情報保護の実装方針を記述する -->
<!-- セキュリティ上の要求レベルは 02_REQUIREMENTS_DEFINITION.md に記載する -->
<!-- 初学者向けの基本: APIキーやトークンなどの秘密情報をコードや画面に直接書かない。入力値をそのまま信用せずチェックする。詳しくは ../../01_ai_basics/ai_safety_basic.md も参照 -->

| Type（種別） | Design Specification（設計仕様） |
|---|---|
| Authentication（認証） | （記入欄） |
| Authorization（認可） | （記入欄） |
| Access Control（権限管理） | （記入欄） |
| Communication（通信） | （記入欄） |
| Data Storage（データ保存） | （記入欄） |
| Data Disposal（データ廃棄） | （記入欄） |
| Personal Data Protection（個人情報保護） | （記入欄） |

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
