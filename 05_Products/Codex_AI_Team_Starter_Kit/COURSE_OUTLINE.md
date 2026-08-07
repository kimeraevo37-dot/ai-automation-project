# 初心者向け Codex AIチーム構築スターターキット — 教材目次

## 1. 教材概要

- **商品名:** 初心者向け Codex AIチーム構築スターターキット
- **想定読者:** ChatGPTの基本操作はできるが、Codex・GitHubは初心者で、Windowsパソコンを使い、AIを副業・個人制作・業務効率化へ活用したい一人。
- **到達目標:** 購入者が、自分のリポジトリで基盤3文書を作成・保存し、CodexへREADME.md一件だけを依頼して、差分確認・2段階のCommit・Push・ブラウザ確認までを人間の承認付きで行える。
- **想定所要時間:** 初版での仮目安。画面確認やアカウント状態により変わるため、確定値ではない。
- **必要な環境:** Windowsパソコン、インターネット環境、GitHubアカウント、GitHub Desktop、Codexを利用できる環境。
- **教材形式:** 日本語の画面付き手順教材、Markdownテンプレート、コピー用プロンプト、チェックリスト、トラブルシューティング、FAQ。

## 2. 学習順序

本編はChapter 0からChapter 11まで順番に進める。飛ばしてはいけない章は、Chapter 3、Chapter 5〜8、Chapter 10である。

1. Chapter 0〜2で役割・環境・安全上の前提をそろえる。
2. Chapter 3で正しいリポジトリを確認する。
3. Chapter 4〜7でフォルダと基盤3文書を作る。
4. Chapter 8で基盤3文書を第1Commit・Pushとして保存する。
5. Chapter 9〜10でREADME.mdだけを第2Commit・Pushとして保存する。
6. Chapter 11で次回の再開方法を残す。
7. 問題が起きた場合だけ、トラブルシューティングを参照する。

## 3. 章別設計

| 章 | 目的 | 扱う内容 | 使用するテンプレート | 必要な画面 | 完了条件 |
| --- | --- | --- | --- | --- | --- |
| Chapter 0：この教材の使い方 | 安全に一つずつ進める前提を理解する | 対象者、完成イメージ、人間とCodexの役割、問題時はCommit・Pushを止めること | なし | 教材全体の進行図 | 購入者が人間の承認が必要な操作を説明できる |
| Chapter 1：CodexとGitHubの全体像 | 今回必要な用語と役割を最小限理解する | Codex、GitHub、GitHub Desktop、リポジトリ、Changes、Commit、Push、ブラウザ版GitHub | なし | Codex・GitHub Desktop・GitHubの役割図 | 3つのツールの役割とCommit・Pushの違いを説明できる |
| Chapter 2：環境を準備する | 作業環境と公開範囲を安全に準備する | GitHubアカウント、GitHub Desktop、新規またはテスト用リポジトリ、Codexとの連携、Private設定、認証情報を公開しない注意 | なし | GitHubのリポジトリ作成画面、GitHub Desktopのサインイン・追加画面 | 対象リポジトリをGitHub Desktopで開ける |
| Chapter 3：正しいリポジトリを確認する | 別リポジトリで作業する事故を防ぐ | Current repository、リポジトリ名、ローカルパス、本番とテスト用の区別、Codexが見るフォルダ、開始前チェック | なし | Current repository、ローカルパス、GitHub URL | 人間とCodexが同じリポジトリ名・パス・ブランチを確認できる |
| Chapter 4：最小フォルダ構成を作る | 作業場所を最小構成で整える | 各フォルダの役割、AGENTS.mdの配置、空フォルダ、`.gitkeep`が必須ではない理由 | `FOLDER_STRUCTURE.md` | エクスプローラーの最小フォルダ構成、GitHub表示との比較 | 必要なフォルダと基盤3文書の保存先を説明できる |
| Chapter 5：ROADMAP.mdを作る | 最優先成果物と進行方針を決める | ROADMAPの目的、最優先成果物一つ、現在のフェーズ、範囲、完了条件、作成依頼の考え方 | `ROADMAP_TEMPLATE.md` | ROADMAP入力例 | ROADMAP.mdに目的・優先順位・完了条件がある |
| Chapter 6：COMPANY_RULE.mdを作る | 人間とCodexの権限を分ける | 承認が必要な操作、Commit・Push、公開・送信・課金、個人情報・認証情報、停止条件 | `COMPANY_RULE_TEMPLATE.md` | COMPANY_RULE入力例 | Push・公開・認証情報の扱いを人間が決めるルールがある |
| Chapter 7：AGENTS.mdを作る | Codexが毎回読む作業ルールを置く | ルート直下へ置く理由、読み順、標準作業手順、報告形式、一度に大量の作業を頼まないルール | `AGENTS_TEMPLATE.md` | ルート直下のAGENTS.md、フォルダ構成 | AGENTS.mdがルート直下にあり、関連文書のパスが正しい |
| Chapter 8：基盤3文書を保存する | 基盤3文書を第1Commitとして安全に保存する | Changesで3ファイルを確認、個人情報確認、Summary、Commit、Push origin、ブラウザ確認、Changesが空である確認 | `COMPANY_RULE_TEMPLATE.md`、`AGENTS_TEMPLATE.md` | 3ファイルだけのChanges、Summary、Push origin、ブラウザ版GitHub | `AGENTS.md`、ROADMAP.md、COMPANY_RULE.mdだけを`docs: プロジェクト基盤を追加`で保存できる |
| Chapter 9：Codexへ最初のタスクを依頼する | README.md一件だけを安全に依頼する | FIRST_TASK_PROMPTの使い方、既存README確認、作業範囲を広げない、Codexの報告確認 | `FIRST_TASK_PROMPT.md` | Codexへ貼り付けるプロンプト、Codexの報告例 | CodexがREADME.md以外を変更しない依頼を理解できる |
| Chapter 10：README.mdだけを確認して保存する | 第2CommitをREADME.mdだけに分離する | READMEのみのChanges、基盤3文書が未変更、内容確認、Summary、Commit、Push、ブラウザ確認 | `FIRST_TASK_PROMPT.md` | README.mdだけのChanges、第2Commit、GitHubの履歴 | README.mdだけを`docs: プロジェクトREADMEを追加`で保存できる |
| Chapter 11：次回の再開方法 | 中断後も同じプロジェクトを再開できるようにする | 対象リポジトリ、ROADMAP、COMPANY_RULE、AGENTS、Git状態、次の小タスク、再開位置の記録 | `ROADMAP_TEMPLATE.md`、`AGENTS_TEMPLATE.md` | 再開時の確認チェックリスト | 次回に読む順序と次の一件のタスクが分かる |

## 4. 正常フローとトラブル情報の分離

### 本編に置く内容

- 正しいリポジトリ・ローカルパスの確認
- 基盤3文書の作成と第1Commit・Push
- README.md一件の依頼と第2Commit・Push
- ブラウザ版GitHubでの反映確認
- 次回の再開方法

### トラブル集へ置く内容

- Changesに予定より多くのファイルが表示される
- 空フォルダがGitHubに表示されない
- CodexがCommitを確認できない
- CodexとGitHub Desktop・ブラウザ版GitHubの表示が違う

### FAQへ置く内容

- `.gitkeep`は必要か
- CodexにCommitさせてもよいか
- PublicとPrivateのどちらがよいか
- 間違ったリポジトリを開いた場合はどうするか
- README.md以外もChangesへ表示された場合はどうするか
- GitHubにフォルダが表示されない理由

### 開発ログだけに残す内容

- ROADMAP_TEMPLATEの保存先ずれ
- README.mdだけがChangesに表示される再テストの内部手順
- 原因が未確定のCommit対象・Summary・Push後修正の個別事例

## 5. トラブルシューティングの構成

| 項目 | 確認すること | 安全な案内 |
| --- | --- | --- |
| Trouble 1：Changesに予定より多くのファイルが表示される | 未Commitの基盤文書が残っていないか、変更対象は何か | 問題が解決するまでCommitせず、基盤3文書を先に保存する |
| Trouble 2：空フォルダがGitHubに表示されない | ローカルにフォルダがあるか、フォルダ内にファイルがあるか | 作成失敗ではないと説明し、`.gitkeep`は必要な場合だけ使う |
| Trouble 3：CodexがCommitを確認できない | Current repository、ローカルパス、Commit・Push後の状態 | 人間とCodexで同じリポジトリ・ブランチを確認してから再開する |
| Trouble 4：CodexとGitHub Desktopの表示が違う | ローカルGit、GitHub Desktop、ブラウザ版GitHubの表示 | 原因を断定せず、名前・パス・ブランチ・Changesを分けて確認する |

## 6. 付録の構成

### Appendix A：用語集

リポジトリ、ローカル、リモート、Changes、差分、Commit、Push、Branch、main、Markdown、AGENTS.md、`.gitkeep`、`.gitignore`。

### Appendix B：コピー用テンプレート

`ROADMAP_TEMPLATE.md`、`COMPANY_RULE_TEMPLATE.md`、`AGENTS_TEMPLATE.md`、`FOLDER_STRUCTURE.md`、`FIRST_TASK_PROMPT.md`。

### Appendix C：チェックリスト

作業開始前、第1Commit前、README作成後、第2Commit前、Push後。

### Appendix D：FAQ

`.gitkeep`、CodexによるCommit、PublicとPrivate、誤ったリポジトリ、README以外のChanges、GitHubに表示されないフォルダを扱う。未検証の高度なGit修復は含めない。

## 7. 画面キャプチャの現在状態

正常フロー用Public画像8枚は作成済みで、`Images/`へ配置し、該当ChapterからMarkdownで参照している。撮影時に個人情報・認証情報を除外し、Public版では教材に不要な識別情報を処理した。

| ID | 画面 | 使用章 | 現在の状態 |
| --- | --- | --- | --- |
| S-001 | GitHub DesktopのCurrent repository | Chapter 3 | Public画像作成済み。`Images/S001_current_repository_public.png`をMarkdown参照済み。 |
| S-003 | GitHub DesktopのChanges（基盤3文書） | Chapter 8 | Public画像作成済み。`Images/S003_foundation_changes_public.png`をMarkdown参照済み。 |
| S-004 | GitHub DesktopのSummaryとChanges | Chapter 8 | Public画像作成済み。`Images/S004_summary_and_changes_public.png`をMarkdown参照済み。 |
| S-005 | Commit後のPush origin | Chapter 8 | Public画像作成済み。`Images/S005_push_origin_public.png`をMarkdown参照済み。 |
| S-006 | GitHub上の基盤ファイルの反映確認 | Chapter 8 | Public画像作成済み。`Images/S006_foundation_files_github_public.png`をMarkdown参照済み。`00_Command_Center`は閉じた状態である。 |
| S-007 | GitHub DesktopのChanges（README.mdのみ） | Chapter 10 | Public画像作成済み。`Images/S007_readme_changes_public.png`をMarkdown参照済み。 |
| S-009 | GitHub上のREADME表示 | Chapter 10 | Public画像作成済み。`Images/S009_readme_github_public.png`をMarkdown参照済み。 |
| S-010 | GitHubのCommit履歴 | Chapter 10 | Public画像作成済み。`Images/S010_commit_history_public.png`をMarkdown参照済み。 |

空フォルダ比較、ローカルパス、Codexへ渡すプロンプトなどの追加候補は、未実施のまま`SCREENSHOT_PLAN.md`で管理する。

## 8. 教材本文作成の優先順位

1. **Chapter 0：この教材の使い方** — 承認・停止・一件ずつ進める前提を最初に置く。
2. **Chapter 3：正しいリポジトリを確認する** — 実際の取り違え経験を正常フローの開始前確認へ変換する。
3. **Chapter 8：基盤3文書を保存する** — 4ファイル表示の問題を防ぐ、最も重要な分岐を具体化する。

## 9. 初版で含めない内容

- 高度なGitコマンド、履歴書き換え、複雑なBranch運用
- APIを使った自動化、SNS自動投稿、SaaS開発
- 収益化ノウハウ、価格設定、法人化
- 複数AIの完全自律運用

## 10. 完成チェックリスト

- [ ] 想定読者が一人に絞られている。
- [ ] 到達点が明確である。
- [ ] 正常フローが一本道になっている。
- [ ] 本編へトラブル情報を詰め込みすぎていない。
- [ ] 一次体験が適切な章へ配置されている。
- [ ] 各章に完了条件がある。
- [ ] 必要な画面が特定されている。
- [ ] 未検証情報を断定していない。
- [ ] 商品要件と矛盾していない。
- [ ] Version 0.2の範囲を超えていない。
