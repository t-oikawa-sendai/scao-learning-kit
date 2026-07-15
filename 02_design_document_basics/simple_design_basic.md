# 簡易設計の基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L2-DESIGN |
| Version（バージョン） | 0.1 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L2 一覧](./README.md) / [SIMPLE_DESIGN_TEMPLATE](./templates/SIMPLE_DESIGN_TEMPLATE.md) / [要件の基本](./requirements_definition_basic.md) |

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Goals（学習目標）](#3-learning-goals学習目標)
4. [Main Content（本文）](#4-main-content本文)
5. [Practical Checkpoints（実務上の確認点）](#5-practical-checkpoints実務上の確認点)
6. [Related Materials（関連資料）](#6-related-materials関連資料)
7. [Change History（変更履歴）](#7-change-history変更履歴)

## 1. Purpose（目的）

要件を「どう作るか」に落とす簡易設計の考え方を理解し、AIへ実装を依頼する前の土台を作れるようにする。

## 2. Target Audience（対象読者）

- 要件は整理できたが、作り方の全体像を描けていない初学者

## 3. Learning Goals（学習目標）

- 全体構成・責務・データの流れを軽く整理できる。
- エラー時の扱いとセキュリティ上の注意を意識できる。
- 検証方針を決めてから実装依頼に進める。

## 4. Main Content（本文）

簡易設計とは、要件を「どう作るか」に落とし込む、最小限の設計である。
本格的な設計書ほど詳しくなくてよいが、実装に入る前に整理しておくと迷いが減る。
一方で、実装コードや具体的なクラス構造まで踏み込みすぎない。

### 4.1 全体構成

- どんな部品（画面、処理、保存先など）で構成されるか。
- それぞれがどうつながるか。

### 4.2 コンポーネントの責務

- 各部品が「何を担当するか」を一言で書く。
- 1つの部品に役割を詰め込みすぎていないかを確認する。

### 4.3 データの流れ

- どんなデータを扱うか（例：日付、金額、カテゴリ）。
- データがどこから来て、どこへ保存され、どう表示されるか。

### 4.4 画面または操作フロー

- どんな画面・操作があるか。
- ユーザーの操作から結果までの流れ（入力 → 処理 → 表示）。

### 4.5 外部連携

- 外部のサービスやライブラリと連携するか。
- 連携する場合、何を渡し、何を受け取るか。
- 連携がない場合は「なし」と書いてよい。

### 4.6 エラー時の扱い

- 入力が正しくないときにどうするか。
- 処理に失敗したときに何を表示するか。
- データが壊れないようにどう扱うか。

### 4.7 セキュリティ上の注意

- APIキーやトークンなどの秘密情報を、コードや画面に直接書かない。
- 入力値をそのまま信用せず、チェックする。
- 詳しくは [AI利用時の安全ルール](../01_ai_basics/ai_safety_basic.md) も参照。

### 4.8 検証方針

- 何をもって「正しく動く」と判断するか。
- どの画面・操作を確認するか。
- 実装後に確認する項目を、簡単に決めておく。

### 4.9 AIに実装依頼する前に整理する理由

- 設計があいまいなままAIに頼むと、意図とずれた実装になりやすい。
- 構成・責務・データ・フローを先に整理しておくと、依頼文が具体的になる。
- AIの出力を確認するときの「チェック基準」にもなる。

### 4.10 テンプレートに含まれる他の項目

[SIMPLE_DESIGN_TEMPLATE.md](./templates/SIMPLE_DESIGN_TEMPLATE.md) には、上記に加えて次の項目がある。

- 前提条件（Assumptions）：設計が成り立つ前提。
- 未決事項（Open Issues）：まだ決まっていない設計判断。決まったら更新する。
- 実装への引き継ぎ（Handoff to Implementation）：実装時に特に注意してほしい点や、AIへ実装依頼するときの注意。

なお、このテンプレートは学習用・小規模ポートフォリオ用に、実務版の4設計書（データ・UI・アーキテクチャ・運用）を簡易統合した派生版である。

## 5. Practical Checkpoints（実務上の確認点）

- 全体構成と各部品の責務が整理されているか。
- データの流れと操作フローが分かるか。
- エラー時の扱いとセキュリティ上の注意を書いたか。
- 検証方針を決めたか。
- 実装コードや具体的クラス構造へ踏み込みすぎていないか。

## 6. Related Materials（関連資料）

- [L2 一覧に戻る](./README.md)
- [SIMPLE_DESIGN_TEMPLATE.md](./templates/SIMPLE_DESIGN_TEMPLATE.md)
- [要件の基本](./requirements_definition_basic.md)
- [AI利用時の安全ルール](../01_ai_basics/ai_safety_basic.md)

## 7. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | 2026-07-15 | Initial draft（初版作成） | Takashi Oikawa |
