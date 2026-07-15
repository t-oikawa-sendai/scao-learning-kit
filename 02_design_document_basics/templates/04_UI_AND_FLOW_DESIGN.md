<!-- このファイルはテンプレートです。コピーして、各項目を自分のプロジェクトの内容に書き換えて使ってください。 -->
<!-- 未確定の項目は、空欄のままか「未確定」と書き、推測を事実として書かないこと。 -->
<!-- 本テンプレートは学習用・小規模ポートフォリオ用の派生版です。ファイル名・責務は正本と一致させています。実務版の正本は solacom_main/docs/standards/templates/design/04_UI_AND_FLOW_DESIGN.md を参照してください。 -->
<!-- ここでは画面・操作フロー・UI層の入力チェックやエラー表示を扱います。データ・個人情報は 03、技術構成は 05、運用・検証は 06 で扱います。 -->

# UI and Flow Design（UI・フロー設計）

<!-- Document Info（文書情報） -->
| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | （記入例: PRJ-UI。PRJ を自分のプロジェクト略号に置き換える） |
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
<!-- どんな画面・操作があり、入力 → 処理 → 表示がどう流れるかを整理する -->
<!-- 画面を持たない場合: 「本文書では対象外。理由: 画面を持たないため」と記載する -->

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

### 5.1 Screen List — Detail Definition（画面一覧・詳細定義）

<!-- 画面名・各画面の入出力項目・レイアウト・操作を含む詳細定義を記載する -->
<!-- 画面名・利用目的の概要は 02_REQUIREMENTS_DEFINITION.md に記載する -->

| Screen ID（画面ID） | Screen Name（画面名） | Input Items（入力項目） | Output Items（出力項目） | Main Operations（主要操作） | Notes（備考） |
|---|---|---|---|---|---|
| SCR-001 | （記入欄） | （記入欄） | （記入欄） | （記入欄） | （記入欄） |

### 5.2 Screen Transition and Business Flow（画面遷移図・業務フロー）

<!-- 画面間の遷移と、ユーザーの操作から結果までの流れ（入力 → 処理 → 表示）を記述する -->
<!-- Mermaid / 画像 / リンクのいずれかで添付する -->

```
（画面遷移図・業務フローを記述、または画像リンクを貼る）
```

### 5.3 Wireframes and Layout Policy（主要画面のワイヤーフレーム・レイアウト方針）

<!-- 各画面のレイアウト方針を記述する。ワイヤーフレームは画像・Figmaリンク・テキスト図のいずれかで添付する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

#### [Screen Name（例: SCR-001）]

（ワイヤーフレーム・レイアウト方針を記述）

### 5.4 Operation Flow and User Scenarios（操作フロー・ユーザーシナリオ）

<!-- 主要なユーザー操作の流れをシナリオ形式で記述する -->

| Scenario ID（シナリオID） | Operation Name（操作名） | Steps（操作手順） |
|---|---|---|
| SC-001 | （記入欄） | 1. （記入欄） → 2. （記入欄） → 3. （記入欄） |

### 5.5 Validation and Error Handling Policy（バリデーション・エラーハンドリング方針 / UI層）

<!-- 入力値のバリデーションルールとエラー表示方針を記述する -->
<!-- 初学者向けの観点: 入力が正しくないときにどうするか、処理に失敗したときに何を表示するか -->
<!-- データが壊れないための扱いは 03_DATA_AND_SECURITY_DESIGN.md も参照する -->

| Target（対象） | Validation Rules（バリデーションルール） | Error Message / Display Policy（エラーメッセージ・表示方針） |
|---|---|---|
| （記入欄） | （記入欄） | （記入欄） |

### 5.6 Accessibility and Responsive Design Policy（アクセシビリティ・レスポンシブ対応方針）

<!-- アクセシビリティ基準・対応ブレークポイント・対応デバイス（例: スマートフォンでも表示が崩れない）を記述する -->
<!-- 該当内容がない場合: 「本文書では対象外。理由: ○○」と記載する -->

（記入欄）

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
