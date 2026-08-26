# LITM（Lost in the Middle）と文脈管理

> **[発展]** 基礎文書でLITMの概要を理解した後、長いContextを扱う必要がある場合に読む。

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-L1-LITM |
| Version（バージョン） | 0.4 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [01 一覧](./README.md) / [生成AI利用の基礎 -202608-](./generative_ai_usage_overview.md) / [移行テンプレート](./migration_context_template.md) |

---

## 1. Purpose（目的）

長いContextで重要情報の扱われ方が変わるLITMの研究結果を踏まえ、長い会話・資料・作業を扱うときの文脈管理方法を理解する。

---

## 2. LITMとは

LITM（Lost in the Middle）は、長い入力の中で重要情報の位置によってモデル性能が変化する現象を扱った研究である。

Liuらの研究では、複数文書QAとKey-Value Retrievalで、関連情報が入力の中間にある場合に性能が大きく低下する傾向が確認された。先頭や末尾の情報が比較的利用されやすい一方、中間情報の利用が弱くなる場合がある。[TACL原論文](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00638/119630/Lost-in-the-Middle-How-Language-Models-Use-Long)

これは「長いContextでは必ず中間を忘れる」という絶対法則ではない。モデル、タスク、Context構造によって結果は変わるため、**長いContextでは重要情報が常に同じ精度で使われるとは限らない**というリスクとして理解する。

---

## 3. 長いContextで起こりやすい問題

- 会話の途中で決めた制約が後続回答へ十分反映されない。
- 大量の資料を渡した結果、重要事項と補助情報の区別が弱くなる。
- 過去の誤った前提もContextへ残り、その後の回答へ影響する。
- 「前に伝えたから使われるはず」という前提で作業を続けると、ずれに気付きにくい。

---

## 4. 文脈管理の方法

### 4.1 重要事項を必要な時点で再提示する

目的、変更禁止範囲、確定仕様など、現在の判断に必要な情報は短く再提示する。

すべての過去情報を繰り返すのではなく、**現在の判断に必要な情報だけを再提示する**。

### 4.2 確定事項をChatだけに置かない

決定事項、仕様、現在状態をREADME、SPEC、設計書、Project Note等へ移す。

Chatを正本にせず、現在有効な情報を文書から再読できる状態にする。

### 4.3 一度に扱う範囲を整理する

大量の課題を一度に依頼するより、目的や成果物の単位で分ける。

ただし、高性能モデルに細かな処理手順まで固定することとは別である。**作業範囲を整理すること**と**解決方法を縛ること**を混同しない。

### 4.4 長大化したら新しいChatへ移行する

会話が長くなり、前提・決定事項・現在地点の追跡が難しくなった場合は、[AI専用・新チャット文脈移行プロトコル](./migration_context_template.md) を使って新しいChatへ移行する。

---

## 5. Practical Checkpoints（確認点）

- 現在の判断に必要な前提が明示されているか。
- 古い情報と現在有効な情報を区別できるか。
- 重要な決定をChatだけに残していないか。
- 長いContextを「全部覚えているはず」と扱っていないか。
- 新しいChatへ移した方が情報を整理できないか。

---

## 6. Evidence

- **EV-005**：[Lost in the Middle: How Language Models Use Long Contexts](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00638/119630/Lost-in-the-Middle-How-Language-Models-Use-Long)

Repository全体のEvidence一覧は [EVIDENCE.md](../EVIDENCE.md) を参照する。
