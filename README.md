# SCAO Learning Kit（学習用資料集）

**[Evidence Last Verified: 2026-08-26](./EVIDENCE.md)**

技術的事実、生成AIの特性、製品仕様、利用方法に関する記述は、原則として**公式Documentation、公式発表、一次研究など、確認可能なEvidenceに基づいています。**

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-ROOT-INDEX |
| Version（バージョン） | 0.9 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [01：AI利用の基礎](./01_ai_basics/README.md) / [02：PF設計・ドキュメント](./02_design_document_basics/README.md) / [03：AIを活用したPF作成](./03_portfolio_creation_guide/README.md) / [EVIDENCE.md](./EVIDENCE.md) / [CHANGELOG.md](./CHANGELOG.md) |

> 詳細な変更履歴は [CHANGELOG.md](./CHANGELOG.md) を参照。

---

## Table of Contents（目次）

1. [Project Overview（概要）](#1-project-overview概要)
2. [Purpose（目的）](#2-purpose目的)
3. [Learning Structure（学習構造）](#3-learning-structure学習構造)
4. [Learning Materials（学習用資料）](#4-learning-materials学習用資料)
5. [Recommended Flow（推奨利用順）](#5-recommended-flow推奨利用順)
6. [Scope（対象範囲）](#6-scope対象範囲)
7. [Evidence Policy（Evidence方針）](#7-evidence-policyevidence方針)
8. [Glossary（用語集）](#8-glossary用語集)
9. [Document Owners and Reviewers（管理者・レビュアー）](#9-document-owners-and-reviewers管理者レビュアー)

---

## 1. Project Overview（概要）

SCAO Learning Kit は、主にIT初学者が、生成AIを活用してポートフォリオ（PF）を設計・実装・完成させるための学習用資料集である。

Repository全体はPF作成を中心に整理する。一方、`01_ai_basics/` はPF・開発用途だけに限定せず、職業訓練校の生徒が学習・就職活動・PF作成・ソフトウェア開発などで生成AIを利用するための共通基礎を扱う。

企業の本番開発手順を完全再現するものではないが、要求・要件・設計・データ・セキュリティ・テスト・レビュー・ドキュメント管理など、実務で重要になる考え方をPF作成に必要な範囲で取り入れる。

---

## 2. Purpose（目的）

初学者がPF作成および日常的な生成AI利用で次の状態に到達することを目的とする。

- 生成AIをどのような場面で利用できるか理解できる。
- 生成AIに何を任せ、何を人間が判断・確認すべきか理解できる。
- Hallucination、迎合、文脈上の制約、秘密情報などのリスクを理解できる。
- 使用するモデルの能力に応じて、指示の粒度を調整できる。
- 実装前に要求・要件・設計を整理できる。
- 設計書テンプレートを使い、設計情報を文書として管理できる。
- 生成AIを使って要求整理、設計書作成、実装指示、テスト、レビューを進められる。
- 最終的に、設計内容と実装内容を説明できるPFを完成させられる。

---

## 3. Learning Structure（学習構造）

本Repositoryは難易度Levelではなく、PF作成時の利用目的を中心に3領域で構成する。

```text
SCAO Learning Kit
│
├─ 01 AIを理解して使う
│  ├─ 生成AI利用の全体像
│  ├─ 安全に利用する
│  ├─ AIへの指示方法
│  ├─ [発展] 生成AIの特性・問題を深掘りする
│  └─ [補助資料] 必要な場面で使う
│
├─ 02 PFを設計・管理する
│  ├─ 要求
│  ├─ 要件
│  ├─ 設計
│  ├─ 設計書テンプレート
│  └─ ドキュメント管理
│
└─ 03 AIを使ってPFを作る
   ├─ AIを活用した要求・要件整理
   ├─ AIを活用した設計書作成
   ├─ AIへの実装指示
   ├─ AI支援を利用した実装
   ├─ テスト・レビュー
   └─ PF完成・公開
```

3領域は独立した教材ではなく、PF完成までを支える役割分担である。

---

## 4. Learning Materials（学習用資料）

### 01：AI利用の基礎

[01_ai_basics/README.md](./01_ai_basics/README.md)

職業訓練校の生徒が、学習・就職活動・PF作成・ソフトウェア開発などで生成AIを利用するための共通基礎を扱う。

最初に読む基礎資料：

1. [生成AI利用の基礎 -202608-](./01_ai_basics/generative_ai_usage_overview.md)
2. [生成AI利用時の安全ルール](./01_ai_basics/ai_safety_basic.md)
3. [生成AIへの指示方法](./01_ai_basics/how_to_instruct_generative_ai.md)

詳細な特性・問題は `[発展]`、必要な場面で使うテンプレートは `[補助資料]` として分離する。

### 02：PF設計・ドキュメント

[02_design_document_basics/README.md](./02_design_document_basics/README.md)

PFを作り始める前に、目的・要求・要件・設計を整理し、設計情報を文書として管理する方法を扱う。

主な内容：

- READMEの基本
- 要求の基本
- 要件の基本
- 簡易設計の基本
- ドキュメント管理の基本
- 設計ドキュメント標準の7ファイル構成テンプレート

設計テンプレートのファイル名と7ファイル構成は固定し、勝手に削減・統合・renameしない。

### 03：AIを活用したPF作成

[03_portfolio_creation_guide/README.md](./03_portfolio_creation_guide/README.md)

01と02で学んだ内容を、実際のPF作成工程へつなげる領域である。

主な対象：

- AIを活用した要求・要件整理
- AIを活用した設計書作成
- AIへの実装指示
- AI支援を利用した実装
- テスト・レビュー
- README・GitHub・公開・提出までの完成工程

この領域は現在整備中である。

---

## 5. Recommended Flow（推奨利用順）

PF作成を始める場合は、次の順序を基本とする。

```text
01 AI利用の基礎
        ↓
02 PF設計・ドキュメント
        ↓
03 AIを活用したPF作成
        ↓
PF完成・公開・説明
```

すべての資料を最初から順番に読む必要はない。必要な資料を参照しながらPF作成を進める。ただし、生成AIへ実装を指示する前に、少なくとも生成AI利用時の安全ルールと要求・要件・設計の基本は確認することを推奨する。

---

## 6. Scope（対象範囲）

### 対象

- IT初学者
- 職業訓練校生
- 独学でPFを作成する人
- 生成AIを学習・就職活動・PF作成・小規模開発で利用する人

### 現在の初版対象外

- AIエージェントを中心とした自律・半自律開発
- Claude Code、Codex等の個別エージェント製品を中心とした高度な運用
- Harness Engineering等の発展的なAI開発運用

これらはLearning Kitの主要部分完成後に発展編として検討する。

### 学習用資料としての位置づけ

- 本Repositoryは実務開発フレームワークそのものではない。
- SCAO本体の導入を前提としない。
- SCAOの設計思想のうち、初学者のPF作成に有効な考え方を学習用に取り入れる。
- 秘密情報、APIキー、パスワード、トークン、秘密鍵、不要な個人情報を教材例やGitへ記載しない。

---

## 7. Evidence Policy（Evidence方針）

技術的事実、生成AIの特性、製品仕様、利用方法に関する記述は、原則として公式Documentation、公式発表、一次研究など、確認可能なEvidenceに基づく。

- 一次情報を優先する。
- 二次情報だけで技術的事実を確定しない。
- 一次情報で確認できない内容は、原則として技術的事実として教材へ記載しない。
- 教材としての説明順・分類・SCAO独自の運用判断は、外部Evidenceと混同せずRepository内の正本で管理する。
- 各教材末尾に、その教材で使用した主要Evidenceを掲載する。
- Repository全体の外部Evidence一覧は [EVIDENCE.md](./EVIDENCE.md) を正本とする。

---

## 8. Glossary（用語集）

### SCAOとは

SCAO（SPEC-Core Architecture - O）は、人間が定めたSPECを中心に、複数の生成AIへ調査・設計・実装・レビューの役割を分担させる開発方式である。

本Learning KitはSCAO本体ではなく、その考え方の一部を初学者向けのPF作成教材として利用する。

| Term（用語） | Definition（定義） |
|---|---|
| PF | Portfolio（ポートフォリオ）。学習成果・設計・実装・説明を示すための成果物。 |
| 生成AI | 利用者の入力やContextを基に、文章・コード・画像等を生成するAIシステム。 |
| LLM | 大規模言語モデル。現在の生成AIを支える主要技術の一つ。 |
| 指示 | 生成AIへ与える要求全体。目的・前提・対象範囲・制約・出力形式・完了条件などを含む。 |
| Prompt | 指示や質問、データなど、生成AIへ実際に入力する内容。 |
| Context | AIが回答・処理を行う際に参照する会話履歴、資料、指示、Tool結果などの情報。 |
| LITM（Lost in the Middle） | 長いContextの中間にある重要情報の利用性能が低下する場合がある現象。 |
| 要求（Request） | 何を達成したいか、なぜ必要かを整理したもの。 |
| 要件（Requirements） | システムが満たすべき条件を整理したもの。 |
| 設計（Design） | 要求・要件を、どのような構造・データ・画面・処理・運用で実現するか整理したもの。 |
| 正本（Canonical Document） | 現在有効な情報として扱う基準文書。 |

---

## 9. Document Owners and Reviewers（管理者・レビュアー）

| Role（役割） | Name（氏名） | Scope（担当範囲） |
|---|---|---|
| Owner（管理者） | Takashi Oikawa | 全学習用資料（All Materials） |
| Reviewer（レビュアー） | 未定（TBD） | 全学習用資料（All Materials） |
