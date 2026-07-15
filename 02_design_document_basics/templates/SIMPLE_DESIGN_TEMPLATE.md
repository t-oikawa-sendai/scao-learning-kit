<!-- このファイルはテンプレートです。コピーして、各項目を自分のプロジェクトの内容に書き換えて使ってください。 -->
<!-- 未確定の項目は、空欄のままか「未確定」と書き、推測を事実として書かないこと。 -->

# 簡易設計（Simple Design）

> 本テンプレートは学習用・小規模ポートフォリオ用であり、実務版ではデータ・UI・アーキテクチャ・運用設計を個別文書（03_DATA_AND_SECURITY_DESIGN / 04_UI_AND_FLOW_DESIGN / 05_ARCHITECTURE_DESIGN / 06_OPERATION_AND_HANDOFF）へ分割する。ここでは4設計書を簡易統合した派生版として1文書にまとめる。実務版の正本は solacom_main/docs/standards/templates/design/ を参照すること。
>
> 実装コード・具体的なクラス一覧・詳細なメソッド設計・過剰なインフラ設計・不要な分割文書は書かない。

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | （例：PRJ-DESIGN） |
| Version（バージョン） | 0.1 |
| Status（ステータス） | Draft |
| Created Date（作成日） | （作成日 YYYY-MM-DD） |
| Last Updated（最終更新日） | （最終更新日 YYYY-MM-DD） |
| Owner（管理者） | （管理者名） |
| Related Documents（関連文書） | （要件やREADMEへのリンク） |

---

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Scope（対象範囲）](#2-scope対象範囲)
3. [Out of Scope（対象外）](#3-out-of-scope対象外)
4. [Assumptions（前提条件）](#4-assumptions前提条件)
5. [Overall Architecture（全体構成）](#5-overall-architecture全体構成)
6. [Component Responsibilities（コンポーネントの責務）](#6-component-responsibilitiesコンポーネントの責務)
7. [Data Design（データ設計）](#7-data-designデータ設計)
8. [UI / Operation Flow（UI・操作フロー）](#8-ui--operation-flowui操作フロー)
9. [External Integrations（外部連携）](#9-external-integrations外部連携)
10. [Security and Privacy（セキュリティ・個人情報）](#10-security-and-privacyセキュリティ個人情報)
11. [Error Handling（エラー処理）](#11-error-handlingエラー処理)
12. [Verification Policy（検証方針）](#12-verification-policy検証方針)
13. [Open Issues（未決事項）](#13-open-issues未決事項)
14. [Handoff to Implementation（実装への引き継ぎ）](#14-handoff-to-implementation実装への引き継ぎ)
15. [Change History（変更履歴）](#15-change-history変更履歴)

---

## 1. Purpose（目的）

要件を「どう作るか」に落とし、構成・責務・フロー・データ・検証方針を整理する。

## 2. Scope（対象範囲）

<!-- この設計が対象とする範囲を書く -->

（記入欄）

## 3. Out of Scope（対象外）

<!-- 扱わないことを書く。なければ「対象外。理由：○○」と書く -->

（記入欄）

## 4. Assumptions（前提条件）

<!-- 設計が成り立つ前提を書く -->

（記入欄）

## 5. Overall Architecture（全体構成）

<!-- どんな部品（画面・処理・保存先など）で構成され、どうつながるかを書く。図やテキスト図でよい -->

（記入欄）

## 6. Component Responsibilities（コンポーネントの責務）

<!-- 各部品が「何を担当するか」を一言で書く -->

| コンポーネント（Component） | 責務（Responsibility） |
|---|---|
| （記入欄） | （記入欄） |

## 7. Data Design（データ設計）

<!-- 扱うデータ種別と、どこから来てどこへ保存され、どう表示されるかを書く -->

| データ（Data） | 内容（Description） | 保存先（Storage） |
|---|---|---|
| （記入欄） | （記入欄） | （記入欄） |

## 8. UI / Operation Flow（UI・操作フロー）

<!-- どんな画面・操作があるか、入力→処理→表示の流れを書く。画面がない場合は「対象外。理由：○○」 -->

（記入欄）

## 9. External Integrations（外部連携）

<!-- 外部サービス・ライブラリと連携するか。連携する場合は何を渡し何を受け取るか。なければ「なし」または「対象外。理由：○○」 -->

（記入欄）

## 10. Security and Privacy（セキュリティ・個人情報）

<!-- 秘密情報の扱い、入力値の検証、個人情報の扱いを書く。詳しくは L1 の安全ルールを参照 -->

- APIキーやトークンなどの秘密情報を、コードや画面に直接書かない。
- 入力値をそのまま信用せず、チェックする。
- （その他の記入欄）

## 11. Error Handling（エラー処理）

<!-- 入力が正しくないとき・処理に失敗したときの扱い、データが壊れないための方針を書く -->

（記入欄）

## 12. Verification Policy（検証方針）

<!-- 何をもって「正しく動く」と判断するか、どの画面・操作を確認するかを書く -->

（記入欄）

## 13. Open Issues（未決事項）

<!-- まだ決まっていないこと。決まったら更新する -->

| ID | Open Issue（未決事項） | Status（状態） |
|---|---|---|
| TBD-001 | （記入欄） | Open |

## 14. Handoff to Implementation（実装への引き継ぎ）

<!-- 実装時に特に注意してほしい点や、AIへ実装依頼するときの注意を書く。なければ「対象外。理由：○○」 -->

（記入欄）

## 15. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | （作成日 YYYY-MM-DD） | Initial draft（初版作成） | （作成者） |
