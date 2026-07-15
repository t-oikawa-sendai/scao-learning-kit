# 要求の基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L2-REQUEST |
| Version（バージョン） | 0.3 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L2 一覧](./README.md) / [01_REQUEST_DEFINITION.md テンプレート](./templates/01_REQUEST_DEFINITION.md) / [要件の基本](./requirements_definition_basic.md) |

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Goals（学習目標）](#3-learning-goals学習目標)
4. [Main Content（本文）](#4-main-content本文)
5. [Practical Checkpoints（実務上の確認点）](#5-practical-checkpoints実務上の確認点)
6. [Related Materials（関連資料）](#6-related-materials関連資料)

## 1. Purpose（目的）

要求（何を達成したいか）の考え方を理解し、目的側の整理ができるようにする。

## 2. Target Audience（対象読者）

- 作りたいものはあるが、目的を言葉にできていない初学者

## 3. Learning Goals（学習目標）

- 要求は「なぜ・誰の・何を達成したいか」を書くものだと理解する。
- 成功条件と対象範囲・対象外を切り分けられる。
- 要求と要件（実現手段）の違いを説明できる。

## 4. Main Content（本文）

### 4.1 要求とは何か

要求とは、「何を達成したいか」を表したものである。
まだ具体的な機能や技術の話ではなく、「なぜ・何のために作るのか」という段階の整理である。

要求があいまいなまま作り始めると、途中で方向がぶれたり、目的とずれた成果物になりやすい。

### 4.2 要求で整理する内容

要求では、次を中心に整理する。

- なぜ必要か（背景）
- 誰の課題か（利用者と、その困りごと）
- 何を達成したいか（目的）
- 成功条件（何が満たされれば「達成できた」と言えるか）
- 対象範囲（今回やること）
- 対象外（今回やらないこと）

### 4.3 例

- なぜ必要か：手書きの家計簿が続かない。
- 誰の課題か：家計を記録したい自分（個人利用）。
- 何を達成したいか：簡単に入力でき、続けられる家計簿を作る。
- 成功条件：1週間分の支出を、負担なく記録できる。
- 対象範囲：支出の記録と一覧表示。
- 対象外：銀行口座との自動連携。

### 4.4 実現手段を書きすぎない

- 使用技術、画面項目、DBの項目といった「どう実現するか」は、要求の段階では書きすぎない。
- 実現手段は、次の段階である要件・簡易設計で扱う。

### 4.5 要件との違い

- 要求は「何を達成したいか（目的側）」を書く。
- 要件は「システムが満たすべき条件（実現側）」を書く。
- まず要求を固め、その後で要件に落とし込む。

要件については [要件の基本](./requirements_definition_basic.md) を参照。

### 4.6 テンプレートに含まれる他の項目

[01_REQUEST_DEFINITION.md（要求定義テンプレート）](./templates/01_REQUEST_DEFINITION.md) には、上記に加えて次の項目がある。

- 前提条件（Assumptions）：要求が成り立つ前提（例：個人利用、公開しない）。あいまいな前提を先に洗い出す。
- 未決事項（Open Issues）：まだ決まっていないこと。分かる範囲で書き、決まったら更新する。
- 詳細設計への引き継ぎ（Handoff to Detail Design）：後続の要件定義・設計フェーズに伝えたい設計意図や判断経緯。要求を「実現側の条件」に落とすときの手がかりになる。

## 5. Practical Checkpoints（実務上の確認点）

- 「なぜ・誰の・何を達成したいか」が書かれているか。
- 成功条件が、確認できる形で書かれているか。
- 対象範囲と対象外が分かれているか。
- 実現手段（技術・画面項目など）を書きすぎていないか。

## 6. Related Materials（関連資料）

- [L2 一覧に戻る](./README.md)
- [01_REQUEST_DEFINITION.md（要求定義テンプレート）](./templates/01_REQUEST_DEFINITION.md)
- [要件の基本](./requirements_definition_basic.md)
