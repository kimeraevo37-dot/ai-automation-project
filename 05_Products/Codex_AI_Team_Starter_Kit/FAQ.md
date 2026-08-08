# FAQ

## 1. このFAQについて

このFAQは、第三者テスト前に確認できる質問候補をまとめた暫定版です。実際の購入者から頻繁に質問された内容や、初心者が必ず迷う内容を断定するものではありません。

回答は、教材本文または開発・検証中の実体験を根拠にしています。想定外の状態で迷った場合は、操作を続けず、[TROUBLESHOOTING.md](TROUBLESHOOTING.md) を確認してください。

## 2. Repository / Branch

### Current repository の名前が `...` で省略されています。大丈夫ですか？

名前が長い場合は末尾が `...` で省略されることがあります。Current repository が対象リポジトリか、必要に応じてリポジトリ名やローカルパスも確認します。→ Chapter 03

### 間違ったリポジトリを開いているかもしれません。どうすればいいですか？

そのまま進めません。Current repository、ローカルパス、branch を確認し、対象のテスト用Privateリポジトリを開き直します。→ Chapter 03、TROUBLESHOOTING.md

### `main` 以外のBranchになっています。進めていいですか？

この教材の正常フローは `main` を前提にしています。`main` でない理由が分からない場合は、CommitやPushをせずに止まります。→ Chapter 03

## 3. Changes / Commit

### Changesに想定外のファイルがあります。どうすればいいですか？

Commitしません。ファイル名と内容を確認し、今回のCommit目的に含まれない場合は、人間が扱いを決めます。→ COMMIT_CHECKLIST.md、TROUBLESHOOTING.md

### README.mdだけのはずなのに、他のファイルもChangesにあります。

README.mdを作る前に基盤3文書をCommitしていない可能性があります。README.mdのCommitへ進まず、基盤3文書の第1Commitが完了しているか確認します。→ Chapter 08、Chapter 10、TROUBLESHOOTING.md

### CommitとPushは何が違いますか？

Commitは確認した変更をパソコン上の履歴へ保存する操作、PushはそのCommitをGitHubへ送る操作です。→ GLOSSARY.md、Chapter 08、Chapter 10

### Summaryには何を書けばいいですか？

今回保存する変更の目的を短く書きます。入力内容がChangesのファイルと一致していることを、Commit前に人間が確認します。→ COMMIT_CHECKLIST.md

### Summaryを間違えてCommitしてしまいました。

まずPush済みかと、ファイル内容に問題がないかを確認します。急いで履歴を書き換えず、状況に応じた対応を人間が判断します。→ TROUBLESHOOTING.md

### Push後にCommitメッセージのミスに気づきました。

追加操作を急がず、GitHub上のCommit履歴とファイル内容を確認します。個人情報や認証情報が関係する場合は、そのまま進めません。→ TROUBLESHOOTING.md

## 4. Push / GitHub

### `Push origin` が表示されています。何を確認してから押せばいいですか？

Current repository と `main` が正しいこと、直前のCommitが意図した内容になっていることを確認します。対象リポジトリやCommit内容に自信がない場合はPushせずに止まります。→ Chapter 08、Chapter 10

### Push後は何を確認すればいいですか？

ブラウザ版GitHubで、対象リポジトリにファイルまたはREADME.mdが反映されたことを確認します。第2Commit後はCommit履歴も確認します。→ Chapter 08、Chapter 10

### GitHub上に空フォルダが表示されません。

作成失敗ではありません。Gitは通常、空のフォルダだけを追跡しないため、フォルダ内にファイルが作られるまでGitHubに表示されない場合があります。→ Chapter 04、TROUBLESHOOTING.md

### `.gitkeep` は必要ですか？

初期構成では必須ではありません。空の状態でもフォルダをGitHubに表示する必要がある場合だけ、変更内容を人間が確認して追加します。→ Chapter 04、TROUBLESHOOTING.md

## 5. Codex

### CodexがREADME.md以外のファイルも変更しました。

CommitやPushへ進めません。Changesで変更ファイルを確認し、依頼内容と違う変更がある場合は、Codexへ状況確認を依頼します。→ Chapter 09、TROUBLESHOOTING.md

### Codexの説明とGitHub Desktopの状態が一致しません。

次のCommitやPushを止めます。GitHub Desktopで開いているリポジトリ、Codexが参照しているローカルフォルダ、ブラウザ版GitHubを分けて確認し、リポジトリ名、ローカルパス、branch、Changesまたは履歴を照合します。→ TROUBLESHOOTING.md

### CodexにCommitやPushを任せてもいいですか？

この教材では任せません。Codexはファイル作成・状態確認・報告を担当し、人間が差分確認、Summary確認、Commit、Pushを行います。→ Chapter 00、Chapter 08、Chapter 10

## 6. 再開

### 次回は何から確認すればいいですか？

リポジトリ名・branch・ローカルフォルダを確認したあと、AGENTS.md、00_Command_Center/ROADMAP.md、00_Command_Center/COMPANY_RULE.md の順で読みます。次にGitの状態と次の1件のタスクを確認します。→ Chapter 11

### 途中で作業を止めても大丈夫ですか？

大丈夫です。迷った状態ではCommitやPushをせず、現在の状態と次に確認するファイルを残してから止めます。→ Chapter 11

## 7. 第三者テスト後に確認する質問候補

次は第三者テストで実際の質問や停止が確認されてから、FAQへ追加または優先順位を判断します。

- `Push origin` が表示されない場合の案内
- 教材とGitHub DesktopまたはGitHubのUIが大きく違う場合の案内
- どのChapterから再開すればよいか判断できない場合の案内
- テスターが用語や画像のどこで止まったかに基づく質問

## 8. 迷ったときの参照先

- 用語の意味 → [GLOSSARY.md](GLOSSARY.md)
- Commit前の短い確認 → [COMMIT_CHECKLIST.md](COMMIT_CHECKLIST.md)
- 想定外の状態 → [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
- 通常の操作手順 → [Course/Chapter 00〜11](Course/)
