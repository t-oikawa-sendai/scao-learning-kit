# AI専用・新チャット文脈移行プロトコル

## [PROJECT_METADATA]
* **PROJECT_NAME**: {{プロジェクト名}}
* **REPOSITORY_URI**: {{リポジトリURL/なし}}
* **LOCAL_WORKSPACE_PATH**: {{ローカル絶対パス}}
* **CURRENT_GIT_BRANCH**: {{ブランチ名}}
* **TARGET_ENVIRONMENT**: {{OS、言語バージョン、DB、IDE等の環境スタック}}

## [KNOWLEDGE_STATE_SNAPSHOT]
### 1. CORE_OBJECTIVE
* {{このチャット、またはタスクが最終的に達成すべき目的}}

### 2. BACKGROUND_AND_PREMISES
* {{前提知識、ビジネス背景、制約条件}}

### 3. FROZEN_SPECIFICATIONS (FACT)
* {{これまでに確定した仕様、アルゴリズム、データ構造。覆してはならない決定事項}}

### 4. COMPLETED_WORK_LOG
* {{これまでに実装・検証が完了した内容。再提案・重複実装を防止するためのログ}}

### 5. CURRENT_SYSTEM_STATUS
* **LAST_COMMIT_HASH**: {{最新コミットハッシュ}}
* **WORKSPACE_STATUS**: {{クリーン / 未コミット変更あり（具体的なファイル名）}}
* **BUILD_STATUS**: {{SUCCESS / FAILED（エラーログ抜粋）}}
* **TEST_STATUS**: {{PASS / FAIL（未解決の失敗テストケース）}}

### 6. IDENTIFIED_ISSUES
* {{現在発生しているバグ、未解決の技術的課題、ボトルネック}}

### 7. SOURCE_FILES_TO_REFERENCE
* {{AIがコンテキスト読み込み時に最優先で参照・解析すべきファイルパスの一覧}}

## [NEXT_ACTION_INSTRUCTION]
* **IMMEDIATE_TASK**: {{翌朝、このプロトコルを読み込んだ直後にAIが実行すべき最初の具体的な指示}}

## [GUARD_RAILS_AND_CONSTRAINTS]
1.  **NO_HALLUCINATION**: 公式仕様や確定ソース（Fact）にない仕様を推測（Inference）で補完してはならない。不明点は即座に質問せよ。
2.  **NO_UNAUTHORIZED_IMPLEMENTATION**: 指示のないコード追加、リファクタリング、および機能拡張を厳禁とする。
3.  **NO_DESTRUCTIVE_CHANGES**: 既存の確定仕様や動作確認済みコードを破壊・退行（デグレード）させる変更を提案・実装してはならない。
4.  **DATA_PRIVACY**: 機密情報、個人情報、認証資格情報を出力に含めてはならない。
