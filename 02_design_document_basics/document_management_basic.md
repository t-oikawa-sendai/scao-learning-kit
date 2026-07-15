# ドキュメント管理の基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L2-DOCMGMT |
| Version（バージョン） | 0.1 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-07-15 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [L2 一覧](./README.md) / [READMEの基本](./readme_basic.md) / [AI利用時の安全ルール](../01_ai_basics/ai_safety_basic.md) |

## Table of Contents（目次）

1. [Purpose（目的）](#1-purpose目的)
2. [Target Audience（対象読者）](#2-target-audience対象読者)
3. [Learning Goals（学習目標）](#3-learning-goals学習目標)
4. [Main Content（本文）](#4-main-content本文)
5. [Practical Checkpoints（実務上の確認点）](#5-practical-checkpoints実務上の確認点)
6. [Related Materials（関連資料）](#6-related-materials関連資料)
7. [Change History（変更履歴）](#7-change-history変更履歴)

## 1. Purpose（目的）

ドキュメントを正しく保つための基本（正本・文書情報・変更履歴・整合性）を理解する。

## 2. Target Audience（対象読者）

- 複数のドキュメントを扱い始め、管理に迷っている初学者

## 3. Learning Goals（学習目標）

- 正本を1つ決め、重複管理を避けられる。
- 文書情報（Version・Status・日付・Owner など）と変更履歴の意味を理解する。
- README・要求・要件・設計の整合性を保つ意識を持つ。

## 4. Main Content（本文）

### 4.1 正本を1つ決める

- 同じ内容のドキュメントが複数あると、どれが正しいか分からなくなる。
- 「これが正しい」という正本（一次情報）を1つ決める。
- 修正するときは、正本を直す。

### 4.2 文書情報（Document Information）

各ドキュメントの先頭に、次のような文書情報を持たせると管理しやすい。

- Version：版番号（例：0.1）。内容を更新したら上げる。
- Status：状態（例：Draft＝下書き、Review＝レビュー中、Approved＝承認済み、Deprecated＝廃止）。
- Created Date：作成日。
- Last Updated：最終更新日。更新したら合わせて直す。
- Owner：管理者（誰が責任を持つか）。
- Related Documents：関連する文書へのリンク。

### 4.3 変更履歴（Change History）

- 「いつ・何を・なぜ変えたか」を残すと、後から追いやすい。
- ポートフォリオでは、細かい履歴管理までは不要なことも多い。
- 大きな変更だけでも記録しておくと、振り返りに役立つ。

### 4.4 重複管理の禁止

- 同じ説明を何箇所にも書くと、片方だけ古くなりやすい。
- 詳細は1箇所（正本）にまとめ、他からはリンクで参照する。
- 古い情報を残しっぱなしにしない。仕様が変わったら更新するか、「廃止」と明記する。

### 4.5 README・要求・要件・設計の整合性

- README（入口）と、要求・要件・簡易設計（詳細）は役割を分ける。
- 各文書の内容が食い違わないようにする（例：要件で消した機能が、READMEに残っていないか）。
- 変更したら、関連する文書もあわせて見直す。

### 4.6 Git履歴と文書記載の整合性

- Gitのコミット履歴と、文書の変更履歴が大きく食い違わないようにする。
- 「文書には更新済みと書いてあるのに、実物は古いまま」を避ける。
- 秘密情報はGit履歴にも残るため、そもそもコミットしない（[安全ルール](../01_ai_basics/ai_safety_basic.md) 参照）。

### 4.7 AIに文書構成を勝手に増やさせない

- AIに依頼すると、頼んでいないドキュメントを新規作成することがある。
- ドキュメントが増えすぎると、管理しきれなくなる。
- 「新しいファイルを勝手に作らないでほしい」と依頼文で明示する。

## 5. Practical Checkpoints（実務上の確認点）

- 正本が1つに定まっているか。
- 文書情報（Version・Status・日付・Owner・Related Documents）があるか。
- 変更履歴が残っているか。
- README・要求・要件・設計の内容が食い違っていないか。
- AIが勝手に文書を増やしていないか。

## 6. Related Materials（関連資料）

- [L2 一覧に戻る](./README.md)
- [READMEの基本](./readme_basic.md)
- [AI利用時の安全ルール](../01_ai_basics/ai_safety_basic.md)

## 7. Change History（変更履歴）

| Version（バージョン） | Date（日付） | Changes（変更内容） | Author（変更者） |
|---|---|---|---|
| 0.1 | 2026-07-15 | Initial draft（初版作成） | Takashi Oikawa |
