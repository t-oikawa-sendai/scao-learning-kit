# L2：設計ドキュメントの基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L2-INDEX |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [トップ](../README.md) / [L1：AI利用の基本](../01_ai_basics/README.md) |

---

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Materials Index（学習用資料一覧）](#3-learning-materials-index学習用資料一覧)
4. [Usage Guide（利用方法）](#4-usage-guide利用方法)
5. [Current Status（現在状態）](#5-current-status現在状態)
6. [Related Materials（関連資料）](#6-related-materials関連資料)
7. [Change History（変更履歴）](#7-change-history変更履歴)

---

## 1. Purpose（目的）

ポートフォリオや小規模アプリを作る前に整理すべき設計ドキュメントの基本を身につける。README、要求、要件、簡易設計、ドキュメント管理を理解し、AIへ実装を依頼する前の土台を作る。

## 2. Target Audience（対象読者）

- 要求・要件・設計の整理が定まっていない初学者
- AIへ実装を依頼する前に、目的と条件を言語化したい人

## 3. Learning Materials Index（学習用資料一覧）

### 解説用の学習用資料

1. [READMEの基本](./readme_basic.md)
2. [要求の基本](./request_definition_basic.md)
3. [要件の基本](./requirements_definition_basic.md)
4. [簡易設計の基本](./simple_design_basic.md)
5. [ドキュメント管理の基本](./document_management_basic.md)

### テンプレート（コピーして使う）

設計テンプレートは、文書標準の正本と同一のファイル名を持つ 7 ファイル構成（README.md + 6 文書）で固定している。初学者向けでもファイルを減らさず、該当しない設計項目は削除せず「対象外。理由：○○」と記載する。

- [README.md（設計書一覧）](./templates/README.md)
- [01_REQUEST_DEFINITION.md（要求定義）](./templates/01_REQUEST_DEFINITION.md)
- [02_REQUIREMENTS_DEFINITION.md（要件定義）](./templates/02_REQUIREMENTS_DEFINITION.md)
- [03_DATA_AND_SECURITY_DESIGN.md（データ・セキュリティ設計）](./templates/03_DATA_AND_SECURITY_DESIGN.md)
- [04_UI_AND_FLOW_DESIGN.md（UI・フロー設計）](./templates/04_UI_AND_FLOW_DESIGN.md)
- [05_ARCHITECTURE_DESIGN.md（アーキテクチャ設計）](./templates/05_ARCHITECTURE_DESIGN.md)
- [06_OPERATION_AND_HANDOFF.md（運用・詳細設計引き継ぎ）](./templates/06_OPERATION_AND_HANDOFF.md)

> ファイル名を正本・全プロジェクトと統一するのは、横断検索・一括置換・文書比較・リンクの安定・レビュー・保守・自動検査を安定させるためである。

## 4. Usage Guide（利用方法）

要求（何を達成したいか）→ 要件（システムが満たすべき条件）→ 簡易設計（どう作るか）の順で整理すると、AIに実装を依頼する前の土台が固まる。READMEとドキュメント管理は、これらを整理・公開するための土台になる。各解説を読んだうえで、対応するテンプレートをコピーして使う。

## 5. Current Status（現在状態）

初版（利用可能）。解説用の学習用資料5点、および設計テンプレート7ファイル（README.md + 6文書）すべて Draft 状態で公開している。

## 6. Related Materials（関連資料）

- [トップに戻る](../README.md)
- [L1：AI利用の基本](../01_ai_basics/README.md)

## 7. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | 2026-07-15 | Initial draft（初版作成）。管理形式準拠のLevel入口READMEへ整備 | Takashi Oikawa |
| 0.2 | 2026-07-15 | 設計テンプレートを独自4ファイル構成から正本準拠の7ファイル構成（README.md + 6文書）へ修正。テンプレート一覧・現在状態・ファイル名統一の目的を反映 | Takashi Oikawa |
