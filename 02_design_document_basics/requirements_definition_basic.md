# 要件の基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L2-REQUIREMENTS |
| Version（バージョン） | 0.2 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L2 一覧](./README.md) / [02_REQUIREMENTS_DEFINITION.md テンプレート](./templates/02_REQUIREMENTS_DEFINITION.md) / [要求の基本](./request_definition_basic.md) / [簡易設計の基本](./simple_design_basic.md) |

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Goals（学習目標）](#3-learning-goals学習目標)
4. [Main Content（本文）](#4-main-content本文)
5. [Practical Checkpoints（実務上の確認点）](#5-practical-checkpoints実務上の確認点)
6. [Related Materials（関連資料）](#6-related-materials関連資料)
7. [Change History（変更履歴）](#7-change-history変更履歴)

## 1. Purpose（目的）

要件（システムが満たすべき条件）の考え方を理解し、実現側の条件を整理できるようにする。

## 2. Target Audience（対象読者）

- 要求は整理できたが、具体的な条件に落とせていない初学者

## 3. Learning Goals（学習目標）

- 機能要件と非機能要件を区別できる。
- 入力・処理・出力の観点で条件を整理できる。
- 受け入れ条件（完了条件）と制約を書ける。

## 4. Main Content（本文）

### 4.1 要件とは何か

要件とは、要求（何を達成したいか）を実現するために、
システムが満たすべき条件を具体的にしたものである。

要求が「目的」だとすれば、要件は「その目的を満たすために必要な条件」である。
要求の背景説明を、ここで重複して長く書く必要はない（背景は要求側に置く）。

### 4.2 機能要件

システムが「何をするか」を表す条件。

- 支出を登録できる
- 登録した支出の一覧を表示できる
- 月ごとの合計を表示できる

### 4.3 非機能要件

「どのように」あるべきかを表す条件。機能そのものではなく、品質や性能に関わる。

- 動作が極端に遅くない
- スマートフォンでも表示が崩れない
- 入力ミスをしてもデータが壊れない

### 4.4 入力・処理・出力

機能を、入力・処理・出力の観点で整理すると、条件の抜けに気づきやすい。

- 入力：何を受け取るか（例：日付、金額、カテゴリ）
- 処理：受け取った入力をどう扱うか（例：保存する、合計する）
- 出力：何を返す・表示するか（例：一覧、合計金額）

### 4.5 制約

作るうえで前提となる制限。

- 使用できる技術や環境
- 期限や作業時間
- 個人利用か、公開するか

### 4.6 受け入れ条件（完了条件）

「どうなったら完成・合格とみなすか」を明確にする。

- すべての機能要件が動作する
- 主要な画面が表示できる
- 明らかなエラーが残っていない

### 4.7 要求との対応

- 各要件は、どの要求を満たすためのものかを意識する。
- 要求に対応しない要件は、過剰になっていないか見直す。
- 要求については [要求の基本](./request_definition_basic.md) を参照。

### 4.8 テンプレートに含まれる他の項目

[02_REQUIREMENTS_DEFINITION.md（要件定義テンプレート）](./templates/02_REQUIREMENTS_DEFINITION.md) には、上記に加えて次の項目がある。

- 前提条件（Assumptions）：要件が成り立つ前提。要求側の前提と重複させず、要件として必要な前提だけを書く。
- 未決事項（Open Issues）：まだ決まっていない条件。決まったら更新する。
- 詳細設計への引き継ぎ（Handoff to Detail Design）：後続の設計・実装フェーズで特に考慮してほしい点。

## 5. Practical Checkpoints（実務上の確認点）

- 機能要件と非機能要件が分かれているか。
- 入力・処理・出力の観点で抜けがないか。
- 受け入れ条件が、確認できる形で書かれているか。
- 要求の背景説明を重複して長く書いていないか。

## 6. Related Materials（関連資料）

- [L2 一覧に戻る](./README.md)
- [02_REQUIREMENTS_DEFINITION.md（要件定義テンプレート）](./templates/02_REQUIREMENTS_DEFINITION.md)
- [要求の基本](./request_definition_basic.md)
- [簡易設計の基本](./simple_design_basic.md)

## 7. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | 2026-07-15 | Initial draft（初版作成） | Takashi Oikawa |
| 0.2 | 2026-07-15 | 設計テンプレートの7ファイル構成化に伴い、テンプレートへのリンクを 02_REQUIREMENTS_DEFINITION.md へ更新し、引き継ぎ項目の説明を正本の章名（詳細設計への引き継ぎ）へ整合 | Takashi Oikawa |
