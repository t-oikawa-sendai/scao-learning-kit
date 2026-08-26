# 生成AI利用時の安全ルール

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L1-SAFE |
| Version（バージョン） | 0.4 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [01 一覧](./README.md) / [生成AI利用の基礎 -202608-](./generative_ai_usage_overview.md) / [生成AIへの指示方法 -202608-](./how_to_instruct_generative_ai.md) |

---

## 1. Purpose（目的）

学習・就職活動・PF作成・ソフトウェア開発などで生成AIを利用するときに、情報漏えい、誤情報の利用、意図しない変更などの事故を避けるための最低限の安全ルールを理解する。

---

## 2. 個人情報・秘密情報は「必要だから全部渡す」にしない

生成AIへ情報を渡す前に、まず**その情報が本当に必要か**を確認する。

- APIキー
- パスワード
- アクセストークン、リフレッシュトークン
- 秘密鍵
- 認証情報
- 企業や学校の機密情報
- 第三者の個人情報

これらは、権限・必要性・利用サービス側のデータ取扱いを確認せず入力しない。

就職活動では、履歴書・職務経歴書など個人情報を含む資料をAIで扱いたい場合がある。その場合も一律に「全部貼る」のではなく、次の順で判断する。

1. その個人情報が処理に本当に必要か確認する。
2. 利用サービスのデータ取扱い・設定を公式情報で確認する。
3. 不要な氏名、住所、電話番号、メールアドレス等は削除またはマスキングする。
4. 第三者情報や企業の機密情報は、権限なしに入力しない。

本資料ではChatGPT、Gemini、Claude等の製品別設定方法までは扱わない。設定は変更されるため、利用時点の公式情報を確認する。

---

## 3. AIの回答をそのまま事実として扱わない

生成AIは、事実と異なる内容をもっともらしく生成することがある。

重要な内容では次を行う。

- 公式Documentation、公式発表、一次研究などで確認する。
- 最新情報が必要な内容では、情報の日付を確認する。
- URL、制度、企業情報、ライブラリ名などは実在確認する。
- AIが自信を持って書いていても、それ自体をEvidenceにしない。

NISTのGenerative AI Profileでも、生成AI固有のリスクを識別し、利用・評価時にリスク管理を行うことが示されている。[NIST公式](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence)

---

## 4. ファイル・画像・ログにも情報は含まれる

情報漏えいは、文章を直接入力する場合だけではない。

### 画面キャプチャ

- 画面端の通知
- ブラウザのタブ
- 環境変数
- 設定ファイル
- メールアドレスや氏名

などが写り込んでいないか、画像全体を確認する。

### ファイル

履歴書、設計書、ログ、設定ファイルなどは、本文以外にも情報を含む場合がある。アップロード前に内容を確認する。

### ログ

エラーログや実行ログには、Token、URL、メールアドレス、内部Pathなどが含まれる場合がある。必要部分だけを共有する。

---

## 5. 開発で生成AIを使う場合

### 5.1 Gitへ秘密情報を入れない

秘密情報は最初からGitへCommitしないことが重要である。

GitHubも、PasswordやToken等がRepositoryへ入った場合は、まず無効化・ローテーションを行い、必要に応じて履歴からの削除を検討するよう案内している。履歴書き換えには副作用があるため、漏えい後の削除より事前防止を優先する。[GitHub公式](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository)

### 5.2 コードやCommandの意味を確認する

- 意味が分からないCommandをそのまま実行しない。
- 削除・上書き・初期化・権限変更を含む処理は特に注意する。
- 変更対象と影響範囲を確認する。

### 5.3 破壊的操作の前に戻せる状態を作る

- Backupなしで削除・初期化・上書きを行わない。
- Git差分や対象Fileを確認する。
- 本番ではなく、安全な環境で先に確認できないか検討する。

---

## 6. Practical Checkpoints（確認点）

生成AIへ情報を渡す前：

- その情報は本当に必要か。
- 不要な個人情報を削除・マスキングしたか。
- 第三者情報・企業秘密を含んでいないか。
- 利用サービスのデータ取扱いを確認したか。

AIの回答を使う前：

- 重要な事実を一次情報で確認したか。
- AIの提案をそのまま実行していないか。
- 変更・実行の影響範囲を理解しているか。
- 破壊的操作ならBackupや復旧方法があるか。

---

## 7. Evidence

- **EV-009**：[OpenAI — GPT-5 System Card](https://deploymentsafety.openai.com/gpt-5)
- **EV-011**：[NIST — Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-generative-artificial-intelligence)
- **EV-012**：[GitHub Docs — Removing sensitive data from a repository](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository)

Repository全体のEvidence一覧は [EVIDENCE.md](../EVIDENCE.md) を参照する。
