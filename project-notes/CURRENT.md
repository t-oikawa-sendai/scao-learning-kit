# CURRENT

Last Updated: 2026-08-24
Status: CURRENT

## PURPOSE

`scao-learning-kit` を、主にIT初学者が生成AIを活用してポートフォリオ（PF）を設計・実装・完成させる際に利用できる学習用資料集として整備する。

本Repositoryの中心は、生成AIそのものを深く研究することではなく、PF作成という具体的な目的に対して、生成AIの基本的な使い方、メリット・デメリット、利用時の注意点、設計ドキュメント、ドキュメント管理、生成AIを活用した設計・実装の進め方を提供することである。

## VERIFIED CURRENT REPOSITORY STATE

2026-08-24時点のGitHub `main` では、Repositoryルートに以下が存在する。

- `README.md`
- `CHANGELOG.md`
- `01_ai_basics/`
- `02_design_document_basics/`
- `03_portfolio_creation_guide/`
- `04_ai_agentic_workflow/`
- `project-notes/`

`04_ai_agentic_workflow/` は物理的には残っているが、現在の初版教材の有効な学習導線からは外している。

## CONFIRMED ACTIVE STRUCTURE

現行の学習構造は難易度Levelではなく、PF作成時の利用目的を中心に次の3領域とする。

1. `01_ai_basics/`：AIを理解して使う
2. `02_design_document_basics/`：PFを設計・管理する
3. `03_portfolio_creation_guide/`：AIを使ってPFを作る

ルート `README.md`、01・02・03各READMEはこの3領域へ整理済みであり、L1〜L4を主構造として扱わない。

## CONFIRMED DESIGN DIRECTION

### 1. AI利用の基礎

PF作成時に生成AIを利用するための基礎として、主に以下を扱う。

- 生成AIの利用方法の基礎
- 生成AIを利用するメリット
- 生成AIを利用するデメリット・限界
- 生成AIを利用するときに気をつけるべきこと

既存の `01_ai_basics/` の9資料は現時点では削除・統合せず維持する。

確認済みの不足：

- 「生成AIのメリット・デメリット・限界」をPF作成の観点で初心者向けに俯瞰する専用資料がまだ存在しない。

### 2. PF設計・ドキュメント

PF作成時に実際に利用できる設計・文書管理資料として、主に以下を扱う。

- READMEの基本
- 要求の基本
- 要件の基本
- 設計の基本
- ドキュメントの管理方法
- 設計書のテンプレート集

既存の `02_design_document_basics/` と配下の設計テンプレート群は、この領域の基礎資産として維持する。

設計テンプレートは次の7ファイル構成を固定する。

- `README.md`
- `01_REQUEST_DEFINITION.md`
- `02_REQUIREMENTS_DEFINITION.md`
- `03_DATA_AND_SECURITY_DESIGN.md`
- `04_UI_AND_FLOW_DESIGN.md`
- `05_ARCHITECTURE_DESIGN.md`
- `06_OPERATION_AND_HANDOFF.md`

### 3. AIを活用したPF作成

`03_portfolio_creation_guide/` は、01と02の教材を実際のPF作成工程へつなぐ役割として再定義した。

現在の基本フロー：

1. テーマ・目的を決める
2. 要求を整理する
3. 要件を整理する
4. 設計書を作成する
5. AIへの実装指示を作る
6. AI支援を利用して実装する
7. テストする
8. レビューする
9. 設計書と実装を整合させる
10. README・GitHub・公開・提出を整える
11. PF完成

03では01・02の説明を重複して書くのではなく、PF作成工程の中で「いつ、どの資料を使うか」を案内する。

## OUT OF CURRENT INITIAL SCOPE

### `04_ai_agentic_workflow/`

`04_ai_agentic_workflow/` は現在の初版整備対象から外す。

理由：

- AIエージェント、Claude Code、Codex、Harness Engineering、半自動ループ等は、PF作成の基礎学習より一段進んだ内容である。
- 初心者向けの初版教材に混在させると、通常の生成AI活用、IDE上のAI支援、AIエージェントの違いが混乱要因になり得る。

扱い：

- 現時点では初版の学習導線から外す。
- 物理削除はまだ行わない。
- Learning Kit主要部分完成後、発展編として追加することを検討する。

## COMPLETED IN CURRENT RESTRUCTURE

- `project-notes/CURRENT.md` を作成し、作業再開地点をRepository内に持たせた。
- ルート `README.md` をPF作成中心の3領域へ再構成した。
- ルートREADMEの現行導線からL1〜L4構造と04の導線を外した。
- `01_ai_basics/README.md` を「利用方法 / 限界・注意事項 / メリット・デメリット」の観点で再整理した。
- `02_design_document_basics/README.md` をPF設計・ドキュメント領域として再整理した。
- `03_portfolio_creation_guide/README.md` をAIを活用したPF作成工程の入口として再設計した。
- 既存教材本文、設計テンプレート、04配下の物理ファイルは変更していない。

## CURRENT WORK

次はREADMEの上位構造ではなく、既存教材本文の棚卸しを行う。

確認対象：

1. `01_ai_basics/` の各資料が、新しい目的に対して必要か、重複していないか、不足がないか。
2. `02_design_document_basics/` の各解説と7テンプレートが、PF作成用途として過不足なくつながっているか。
3. `03_portfolio_creation_guide/` に追加すべき詳細教材を、PF作成工程単位で定義する。

## NEXT ACTION

1. `01_ai_basics/` の全資料を精読し、次の分類で棚卸しする。
   - 残す
   - 内容調整
   - 統合候補
   - 位置づけ変更
   - 不足資料
2. 特に不足している「生成AIのメリット・デメリット・限界」の初心者向け資料の必要内容を定義する。
3. 01の整理が終わった後、02の全資料とテンプレートを同様に棚卸しする。
4. その後、03の詳細教材構成を確定する。

## DO NOT DO YET

- `04_ai_agentic_workflow/` を物理削除しない。
- 既存教材本文を棚卸し前に削除・renameしない。
- 7ファイルの設計テンプレート構成を変更しない。
- 03の詳細教材を、01・02との重複確認前に大量作成しない。
- 高度なAIエージェント運用を初版の主教材へ戻さない。

## RESUME ORDER

新しいチャットまたは作業再開時は、次の順で確認する。

1. `project-notes/CURRENT.md`
2. ルート `README.md`
3. 作業対象ディレクトリの `README.md`
4. 対象資料本文
5. 必要時のみ `CHANGELOG.md`

## REFERENCES

- `README.md`
- `01_ai_basics/README.md`
- `02_design_document_basics/README.md`
- `03_portfolio_creation_guide/README.md`
- `CHANGELOG.md`
