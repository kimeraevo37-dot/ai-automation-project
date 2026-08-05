# Chapter 9：Codexへ最初のタスクを依頼する

## この章の目的

基盤3文書を保存した後、CodexへREADME.md一件だけを安全に依頼します。

## この章で行うこと

- 第1CommitとPushが終わっていることを確認します。
- `FIRST_TASK_PROMPT.md`を使います。
- README.md以外を変更しない依頼をします。

## 手順

1. GitHub DesktopのChangesが空であることを確認します。
2. ブラウザ版GitHubで基盤3文書が見えることを確認します。
3. `FIRST_TASK_PROMPT.md`を開き、入力欄を自分のプロジェクト用に書き換えます。
4. プロンプトをCodexへ貼り付けます。
5. Codexに、AGENTS.md、ROADMAP.md、COMPANY_RULE.md、Git状態、既存README.mdの有無を確認させます。
6. CodexはREADME.mdだけを作成し、Commit・Pushを実行しないことを確認します。
7. Codexの報告を読み、README.md以外を変更していないか確認します。

## よくある間違い

- 基盤3文書が未CommitのままREADMEを作る。Changesに4ファイルが表示されるため、先にChapter 8を完了します。
- README以外のファイル作成も同時に頼む。最初のタスクは一件に限定します。
- 既存README.mdを確認せずに上書きする。存在する場合は、まず内容と改善案を確認します。

## 完了条件

- [ ] 基盤3文書が第1Commit・Push済みである。
- [ ] GitHub DesktopのChangesが空である。
- [ ] CodexへREADME.md一件だけを依頼した。
- [ ] CodexがCommit・Pushを実行していない。

## 次の章

次は、README.mdだけがChangesに表示されていることを確認し、第2Commitとして保存します。
