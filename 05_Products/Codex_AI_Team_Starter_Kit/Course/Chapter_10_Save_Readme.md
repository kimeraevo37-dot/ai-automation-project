# Chapter 10：README.mdだけを確認して保存する

## この章の目的

README.mdだけを確認し、第2Commit・Pushとして保存します。

## この章で行うこと

- ChangesにREADME.mdだけが表示されていることを確認します。
- READMEの内容を確認します。
- 人間が第2Commit・Pushを行い、ブラウザ版GitHubで確認します。

## 手順

1. GitHub DesktopのChangesを開きます。
2. `README.md`だけが表示されていることを確認します。
3. 基盤3文書がChangesに混ざっていないことを確認します。
4. READMEの見出し、目的、構成、再開方法、安全ルールを読みます。
5. Summaryへ次を入力します。

```text
docs: プロジェクトREADMEを追加
```

6. SummaryとREADME.mdだけが一致していることを確認します。
7. 問題がなければ、人間がCommitを実行します。
8. Commit後、人間がPush originを実行します。
9. ブラウザ版GitHubでREADME.mdとCommit履歴を確認します。

> **画像候補：S-007**
> README.mdだけがChangesに表示される画面。
> 読者が確認する箇所：Changes一覧にREADME.mdだけがあること。
> 暫定判定：必須。

> **画像候補：S-009、S-010**
> ブラウザ版GitHubでREADME.mdとCommit履歴を確認する画面。
> 読者が確認する箇所：README表示と、基盤・READMEが別Commitであること。
> 暫定判定：S-009は必須、S-010は補助。

## よくある間違い

- README.md以外のファイルがChangesにあるままCommitする。原因を確認し、Commitを止めます。
- SummaryがREADME用なのに、複数のファイルを含める。SummaryとChangesを読み比べます。
- Push後にブラウザ版GitHubを確認しない。READMEとCommit履歴を確認します。
- Push後に間違いへ気づき、慌てて履歴を書き換える。個人情報・認証情報がない場合でも、まず変更内容を確認してから次の対応を判断します。

## 完了条件

- [ ] ChangesにREADME.mdだけが表示された。
- [ ] READMEの内容を確認した。
- [ ] SummaryとCommit対象が一致している。
- [ ] 人間が第2CommitとPushを実行した。
- [ ] ブラウザ版GitHubでREADME.mdとCommit履歴を確認した。

## 次の章

次は、途中で止まっても同じプロジェクトを再開する方法を確認します。

## 体調や時間に余裕がない日の最小タスク

今日はここまででも大丈夫です。Changesに`README.md`だけが表示されているか確認します。
