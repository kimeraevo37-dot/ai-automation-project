# ここから始めます

このファイルを最初に開いてください。

この教材は、GitHub Desktop と Codex を使い、初心者・非エンジニアが安全な小さな作業の流れを体験するためのスターターキットです。Chapter を上から順に進め、分からない状態で Commit や Push をしないことを大切にします。

## この教材でできること

- 正しいリポジトリと `main` を確認する
- `AGENTS.md`、`ROADMAP.md`、`COMPANY_RULE.md` の基盤3文書を作る
- Changes を確認してから、第1Commit と Push を行う
- Codex へ `README.md` 一件だけを依頼し、第2Commit と Push を行う
- ブラウザ版GitHubでファイルとCommit履歴を確認し、次回の作業を安全に再開する

この教材は、プログラミング能力を試すものではありません。高度なGit操作、履歴の書き換え、自動収益化などは扱いません。

## 対象者

- Git、GitHub、GitHub Desktop をこれから使い始める方
- Codex の利用経験がない、または浅い方
- プログラミング経験がなくても、画面を見ながら一つずつ進めたい方

## 最初に読む場所

次は `Course/Chapter_00_Getting_Started.md` です。Chapter 00 から Chapter 11 まで、原則として番号順に進めてください。

途中の章だけを先に実行すると、確認するファイルやGitの状態がそろわない場合があります。迷ったときは、無理に先へ進まず、このファイルと該当するChapterへ戻ります。

## 必要な環境

- Windows が使えるパソコン
- 利用できるGitHubアカウント
- GitHub Desktop
- Codex
- 練習用のPrivateリポジトリ
- ブラウザ版GitHubを確認できるインターネット接続

最初の練習では、本番の作業用リポジトリではなく、テスト用のPrivateリポジトリを使います。ファイルや画面に、個人情報・認証情報・アクセストークンを書かないでください。

## Courseの進め方

1. Chapter 00〜03で、安全ルール、役割、正しいリポジトリ、`main` を確認します。
2. Chapter 04〜07で、最小フォルダ構成と基盤3文書を作ります。
3. Chapter 08で、基盤3文書だけを確認して第1Commit・Pushを行い、GitHub上で反映を確認します。
4. Chapter 09で、Codexへ `README.md` 一件だけを依頼します。
5. Chapter 10で、`README.md` だけを確認して第2Commit・Pushを行い、GitHubとCommit履歴を確認します。
6. Chapter 11で、次回の再開手順を確認します。

Codexはファイル作成・状態確認・報告を担当します。人間は差分確認、Summary確認、Commit、Push、最終承認を担当します。対象リポジトリ、`main`、Changes、Summaryのどれかに自信がないときは、CommitやPushをせずに止まります。

## Templatesの使い方

`Templates/` には、作業を始めるためのひな型があります。テンプレート原本を直接作業記録にせず、必要なものを自分のテスト用または作業用リポジトリへコピーしてから使います。

- `ROADMAP_TEMPLATE.md`：進め方を整理する
- `COMPANY_RULE_TEMPLATE.md`：人間とCodexの役割・承認ルールを決める
- `AGENTS_TEMPLATE.md`：Codexへの共通指示を用意する
- `FOLDER_STRUCTURE.md`：最小フォルダ構成を確認する
- `FIRST_TASK_PROMPT.md`：最初のCodex依頼を確認する
- `CHANGELOG.md`：自分のプロジェクトでの変更記録を残す

## 困ったときの参照先

現在の開発リポジトリでは付録はルート直下にあり、購入者向け配布時に `Appendix/` へまとめる予定です。通常の操作手順と付録の役割を次のように分けます。

- 用語の意味を確認したい：`Appendix/GLOSSARY.md`
- Commitボタンを押す直前：`Appendix/COMMIT_CHECKLIST.md`
- 短い疑問の最初の確認先：`Appendix/FAQ.md`
- 想定外の状態になった：`Appendix/TROUBLESHOOTING.md`
- 通常の手順へ戻りたい：`Course/Chapter_00_Getting_Started.md` から Chapter 11

別のリポジトリを開いている可能性がある、Changesに想定外のファイルがある、またはCodexが意図しない変更をした場合は、そのまま進めずに止まります。`force push`、`reset --hard`、公開済み履歴の書き換えは、この教材の標準的な解決方法ではありません。

## 更新履歴

購入者向け配布パッケージの更新は、ルートの `CHANGELOG.md` で確認する予定です。これは `Templates/CHANGELOG.md` と別のファイルです。後者は、購入者自身のプロジェクトで使うひな型です。

## 現在の状態とサポート範囲

この教材は、第三者テスト前の版です。第三者テストで確認できた質問、迷いやすい箇所、画面表示の差異は、今後の更新候補として扱います。第三者テストを実施済みとは扱いません。

サポートの範囲、連絡方法、対応時間は、Version 1.0で確定予定です。現時点で個別サポートの内容や回答期限を約束するものではありません。

## 無理なく進めるために

一度に最後まで進める必要はありません。今日は一つの確認だけで止めても大丈夫です。止めるときは、現在のChapter、GitHub DesktopのChangesまたは履歴、次に行う一件を記録しておくと、Chapter 11から安全に再開できます。
