# [補助資料] Markdownの基本

## Document Information（文書情報）

| Item（項目） | Value（値） |
|---|---|
| Document ID（文書ID） | SLK-02-MD |
| Version（バージョン） | 0.4 |
| Status（ステータス） | Draft |
| Created Date（作成日） | 2026-07-15 |
| Last Updated（最終更新日） | 2026-08-26 |
| Owner（管理者） | Takashi Oikawa |
| Related Documents（関連文書） | [02 一覧](./README.md) / [ドキュメント管理の基本](./document_management_basic.md) / [READMEの基本](./readme_basic.md) |

> `[補助資料]`：設計を学ぶための必須教材ではない。READMEや設計書をMarkdownで記述する際、必要に応じて参照する。

---

## 1. Purpose（目的）

READMEや設計書などをMarkdownで記述するために必要な、最小限の記法を理解する。

Markdownの網羅的な仕様を覚えることは目的としない。**文書へ構造を付け、読み手へ伝わりやすくするための記述手段**として扱う。

---

## 2. 基本記法

### 2.1 見出し

`#` の数で見出しの階層を表す。

```markdown
# 大見出し
## 中見出し
### 小見出し
```

### 2.2 箇条書き

```markdown
- 項目A
- 項目B
```

### 2.3 番号付きリスト

```markdown
1. 最初の作業
2. 次の作業
3. 確認
```

### 2.4 チェックリスト

```markdown
- [ ] 未完了
- [x] 完了
```

### 2.5 コードブロック

````markdown
```text
ここにコードやCommandを書く
```
````

### 2.6 表

```markdown
| 項目 | 内容 |
|---|---|
| 目的 | 説明 |
| 状態 | Draft |
```

### 2.7 引用

```markdown
> 注意事項や引用
```

---

## 3. 設計文書での使い分け

- 章立てを示す → 見出し
- 並列の項目を整理する → 箇条書き
- 順序を示す → 番号付きリスト
- 作業状況を確認する → チェックリスト
- Commandやコードを本文と分ける → コードブロック
- 複数項目を比較する → 表
- 注意事項を本文から分ける → 引用

見た目を飾ることが目的ではない。**文書の責務・構造・判断条件を読み手が追いやすくすること**が目的である。

---

## 4. Practical Checkpoints（確認点）

- 見出しの階層が崩れていないか。
- 箇条書きと番号付きリストを目的に応じて使い分けているか。
- コードやCommandを本文と区別できているか。
- 表を使いすぎて横に長くなっていないか。
- Markdown記法そのものが目的になっていないか。

---

## 5. Evidence

- **EV-013**：[GitHub Flavored Markdown Spec](https://github.github.com/gfm/)

Repository全体のEvidence一覧は [EVIDENCE.md](../EVIDENCE.md) を参照する。
