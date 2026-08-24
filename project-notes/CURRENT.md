# CURRENT

Last Updated: 2026-08-24
Status: CURRENT

## PURPOSE

`scao-learning-kit` を、主にIT初心者が生成AIを活用してポートフォリオ（PF）を設計・実装・完成させる際に利用できる学習用資料集として整備する。

本Repositoryの中心は、生成AIそのものを深く研究することではなく、PF作成という具体的な目的に対して、生成AIの基本的な使い方、注意点、設計ドキュメント、ドキュメント管理、生成AIを活用した設計・実装の進め方を提供することである。

## VERIFIED CURRENT REPOSITORY STATE

2026-08-24時点のGitHub `main` では、Repositoryルートに以下が存在する。

- `README.md`
- `CHANGELOG.md`
- `01_ai_basics/`
- `02_design_document_basics/`
- `03_portfolio_creation_guide/`
- `04_ai_agentic_workflow/`

現行READMEではL1〜L4のLevel構成を採用しているが、現在この全体構成をPF作成中心の構造へ見直している。

## CONFIRMED DESIGN DIRECTION

### 1. AI利用の基礎

PF作成時に生成AIを利用するための基礎として、主に以下を扱う。

- 生成AIの利用方法の基礎
- 生成AIを利用するメリット
- 生成AIを利用するデメリット・限界
- 生成AIを利用するときに気をつけるべきこと

既存の `01_ai_basics/` にある資料は、この目的に沿って整理対象とする。

### 2. PF設計・ドキュメント

PF作成時に実際に利用できる設計・文書管理資料として、主に以下を扱う。

- 設計書のテンプレート集
- 要求・要件・設計の基本
- ドキュメントの管理方法

既存の `02_design_document_basics/` と配下の設計テンプレート群は、この領域の基礎資産として扱う。

### 3. AIを活用したPF作成

生成AIを単なる質問ツールとしてではなく、PF作成工程で活用する方法を扱う。

主な対象は以下とする。

- 生成AIを活用した要求・要件整理
- 生成AIを活用した設計書作成
- 生成AIへの実装指示
- AI支援を利用した実装
- テスト・レビュー
- PF完成までの流れ

既存の `03_portfolio_creation_guide/` は、このPF作成全体の利用目的に沿って再整理・拡充する。

## OUT OF CURRENT INITIAL SCOPE

### `04_ai_agentic_workflow/`

`04_ai_agentic_workflow/` は、現在の初版整備対象から外す。

理由：

- AIエージェント、Claude Code、Codex、Harness Engineering、半自動ループ等は、PF作成の基礎学習より一段進んだ内容である。
- 初心者向けの初版教材に混在させると、通常の生成AI活用、IDE上のAI支援、AIエージェントの違いが混乱要因になり得る。

扱い：

- 現時点では「対象外」とするだけであり、物理削除はまだ決定していない。
- `scao-learning-kit` の主要部分完成後、発展編として追加することを検討する。

## CURRENT STRUCTURAL VIEW

現時点の整備方針は、難易度Levelではなく、PF作成時の利用目的を中心に次の3領域で考える。

1. AIを理解して使う
2. PFを設計・管理する
3. AIを使ってPFを作る

既存ファイルを直ちに削除・renameするのではなく、まず既存資料を上記3領域へ整理し、重複・不足・位置づけを確認した上でRepository構造を確定する。

## CURRENT WORK

- Repository内部構造の棚卸し
- 既存資料をPF作成中心の3領域へ再分類
- 現行L1〜L4構成を維持するか廃止するかの検討
- `04_ai_agentic_workflow/` を初版対象から切り離した状態で、01〜03を中心に完成形を設計する

## NEXT ACTION

1. `01_ai_basics/` の全資料を確認し、AI利用の基礎・メリット/デメリット・注意事項という目的に対して、残す資料、統合候補、追加不足を整理する。
2. `02_design_document_basics/` の全資料とテンプレートを確認し、PF作成用の設計・ドキュメント資産として過不足を整理する。
3. `03_portfolio_creation_guide/` に必要なPF作成工程を定義し、AIを活用した設計書作成・実装・テスト・レビュー・完成までの導線を設計する。
4. 1〜3の整理後に、ルートREADMEおよびRepository構造の変更案を確定する。

## DO NOT DO YET

- `04_ai_agentic_workflow/` を物理削除しない。
- 既存資料を根拠なく削除・renameしない。
- L1〜L4表現を整理前に一括置換しない。
- 設計テンプレートの7ファイル構成を勝手に変更しない。

## RESUME ORDER

新しいチャットまたは作業再開時は、次の順で確認する。

1. `project-notes/CURRENT.md`
2. ルート `README.md`
3. 作業対象ディレクトリの `README.md`
4. 対象資料本文
5. 必要時のみ `CHANGELOG.md`

## REFERENCES

- `README.md`
- `CHANGELOG.md`
- `01_ai_basics/README.md`
- `02_design_document_basics/README.md`
- `03_portfolio_creation_guide/README.md`
- `04_ai_agentic_workflow/README.md`
