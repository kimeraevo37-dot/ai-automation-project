# Chapter 1：CodexとGitHubの全体像

## この章の目的

今回の作業に必要な道具と言葉だけを確認します。詳しいGitの仕組みは扱いません。

## この章で行うこと

- Codex、GitHub、GitHub Desktopの役割を分けます。
- リポジトリ、Changes、Commit、Pushの意味を短く確認します。
- 人間とCodexの役割を確認します。

## 手順

1. **Codex**は、指示されたファイルを作り、内容や状態を確認する担当です。
2. **GitHub Desktop**は、パソコン上の変更を確認し、CommitとPushを行うための画面です。
3. **GitHubのブラウザ版**は、Push後にファイルと履歴が反映されたか確認する場所です。
4. **リポジトリ**は、プロジェクトのファイルと変更履歴をまとめる場所です。
5. **Changes**は、まだCommitしていない変更の一覧です。
6. **Commit**は、確認した変更をパソコン側の履歴へ記録する操作です。
7. **Push**は、そのCommitをGitHubへ送る操作です。
8. CodexはCommitとPushを実行しません。人間が差分を確認してから実行します。

## よくある間違い

- Commitしただけで、GitHubのブラウザ版にも反映されたと思う。CommitとPushは別の操作です。
- Codexへ、内容確認なしにCommitやPushを任せる。人間の確認と承認を残します。
- GitHub Desktopとブラウザ版GitHubを同じものとして扱う。前者はローカルの変更、後者はPush後の反映を確認します。

## 完了条件

- [ ] Codex、GitHub Desktop、ブラウザ版GitHubの役割を説明できる。
- [ ] Changes、Commit、Pushの違いを説明できる。
- [ ] CommitとPushは人間が行うことを確認した。

## 次の章

次は、GitHub・GitHub Desktop・Codexを使うための環境を準備します。
