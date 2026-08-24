# 02：PF設計・ドキュメント

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-02-INDEX |
| Version（バージョン） | 0.5 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-24 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [トップ](../README.md) / [01：AI利用の基礎](../01_ai_basics/README.md) / [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md) |

---

## 1. Purpose（目的）

PFを実装する前に、目的・要求・要件・設計を整理し、設計情報をドキュメントとして管理できるようにする。

生成AIへすぐ実装を依頼するのではなく、まず「何を作るのか」「なぜ作るのか」「何を満たす必要があるか」「どう作るか」を整理し、その内容を設計書へ残すことを重視する。

---

## 2. Target Audience（対象読者）

- PFを作りたいが、何から整理すべきか分からない初学者
- 要求・要件・設計の違いを学びたい人
- 生成AIへ実装を指示する前に、目的と条件を言語化したい人
- PFの設計内容を後から説明・修正できる形で残したい人

---

## 3. Learning Structure（学習構造）

### A. 設計の基本を学ぶ

1. [READMEの基本](./readme_basic.md)
2. [要求の基本](./request_definition_basic.md)
3. [要件の基本](./requirements_definition_basic.md)
4. [簡易設計の基本](./simple_design_basic.md)
5. [ドキュメント管理の基本](./document_management_basic.md)

基本の流れは次のとおりとする。

```text
目的・背景
   ↓
要求（何を達成したいか）
   ↓
要件（何を満たす必要があるか）
   ↓
設計（どう実現するか）
   ↓
実装指示
```

### B. 設計書テンプレートを使う

設計テンプレートは、文書標準の正本と同一のファイル名を持つ7ファイル構成（README.md + 6文書）で固定する。

- [README.md（設計書一覧）](./templates/README.md)
- [01_REQUEST_DEFINITION.md（要求定義）](./templates/01_REQUEST_DEFINITION.md)
- [02_REQUIREMENTS_DEFINITION.md（要件定義）](./templates/02_REQUIREMENTS_DEFINITION.md)
- [03_DATA_AND_SECURITY_DESIGN.md（データ・セキュリティ設計）](./templates/03_DATA_AND_SECURITY_DESIGN.md)
- [04_UI_AND_FLOW_DESIGN.md（UI・フロー設計）](./templates/04_UI_AND_FLOW_DESIGN.md)
- [05_ARCHITECTURE_DESIGN.md（アーキテクチャ設計）](./templates/05_ARCHITECTURE_DESIGN.md)
- [06_OPERATION_AND_HANDOFF.md（運用・詳細設計引き継ぎ）](./templates/06_OPERATION_AND_HANDOFF.md)

初学者向けでもファイルを減らさない。該当しない設計項目は削除せず、「対象外」と理由を記録する。

> ファイル名を全プロジェクトで統一するのは、横断検索・比較・リンク・レビュー・保守・自動処理を安定させるためである。

### C. ドキュメントを管理する

設計書は作成して終わりではない。

PF作成中に仕様や設計が変わった場合は、実装だけを変更せず、現在有効な設計内容と実装内容の整合を維持する。

ドキュメント管理の具体的な考え方は [ドキュメント管理の基本](./document_management_basic.md) で扱う。

---

## 4. Usage Guide（利用方法）

1. READMEでPFの目的と全体像を整理する。
2. 要求を整理する。
3. 要件へ落とし込む。
4. データ・セキュリティ、UI・フロー、アーキテクチャ、運用の設計を整理する。
5. 設計内容を正本として維持する。
6. その設計内容を基に生成AIへ実装を指示する。

設計書テンプレートはコピーしてPF Repositoryで利用することを想定する。

---

## 5. Current Status（現在状態）

解説用の学習用資料5点と設計テンプレート7ファイルは、利用可能なDraftとして維持する。

この領域は現在のSCAO Learning Kitの構想と概ね一致しているため、大幅な構造変更は行わない。今後は内容の重複、不足、初学者向け説明の粒度を確認する。

---

## 6. Fixed Rules（固定事項）

- 設計ドキュメントは7ファイル構成を維持する。
- ファイル名を変更しない。
- ファイルの削減・統合・分割・並べ替えを勝手に行わない。
- 該当しない項目があっても文書自体を削除しない。

---

## 7. Related Materials（関連資料）

- [トップに戻る](../README.md)
- [01：AI利用の基礎](../01_ai_basics/README.md)
- [03：AIを活用したPF作成](../03_portfolio_creation_guide/README.md)
