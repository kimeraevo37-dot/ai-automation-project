# スクリーンショット計画 — Version 0.2

## 1. 画面キャプチャの目的

画面キャプチャは装飾ではなく、初心者が次に見る場所と正しい状態を確認するための証拠として使う。

- 文章だけで操作位置が分かる場合は、画面を増やさない。
- 操作位置、正常状態、失敗状態を区別する。
- 撮影時点のUIであり、GitHub・GitHub Desktop・Codexの将来の画面変更を保証しない。
- 公式仕様の説明と、自分のテストで確認した体験を区別する。
- 本番の`AI Automation Project`は撮影元にしない。

## 2. 採用基準

次の一つ以上を満たす場合だけ採用する。

1. 文章だけではボタンや確認位置が分かりにくい。
2. 正常状態と問題状態を比較する価値がある。
3. リポジトリ名・ファイル・Commit対象の確認が重要である。
4. Commit・Push前後の確認状態を示す必要がある。
5. 実際に起きた失敗を、安全に再現または確認できる。
6. 同じ画面を複数章で再利用できる。
7. 個人情報を撮影前に除外でき、教材理解を本当に助ける。

## 3. 画面一覧

| ID | 画面名 | 使用章 | 伝える内容 | 必須度 | 撮影元 | 個人情報リスク | 加工方針 | 状態 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| S-001 | GitHub DesktopのCurrent repository | Chapter 3 | 作業開始前に正しいリポジトリ名を確認する | 必須 | 新しいPrivateテスト用リポジトリ | GitHub名、他リポジトリ名 | 必要箇所だけ切り抜き、他の履歴を隠す | Public版完成。`Images/S001_current_repository_public.png`をMarkdown参照済み。 |
| S-002 | ローカルパスの確認 | Chapter 3、Trouble 3 | CodexとGitHub Desktopが同じフォルダを見ているか確認する | 高 | 新しいPrivateテスト用リポジトリ | Windowsユーザー名、ローカルパス | 架空の安全なユーザー名・パスで撮影できる場合のみ採用 | 再現可否確認中 |
| S-003 | 基盤3文書だけがChangesにある状態 | Chapter 8 | 第1Commit前の対象は3ファイルだけである | 必須 | 新しいPrivateテスト用リポジトリ | ファイル内容、リポジトリ名 | Changes一覧を中心に切り抜く | Public版完成。`Images/S003_foundation_changes_public.png`をMarkdown参照済み。 |
| S-004 | Summary入力欄とChanges | Chapter 8 | SummaryとCommit対象を一緒に確認する | 必須 | 新しいPrivateテスト用リポジトリ | ファイル内容、リポジトリ名 | 3ファイル一覧とSummaryだけを残す | Public版完成。`Images/S004_summary_and_changes_public.png`をMarkdown参照済み。 |
| S-005 | Push originが表示された状態 | Chapter 8 | CommitとPushは別操作で、人間がPushする | 必須 | 新しいPrivateテスト用リポジトリ | アカウント名、通知 | ボタン周辺だけを切り抜く | Public版完成。`Images/S005_push_origin_public.png`をMarkdown参照済み。 |
| S-006 | ブラウザ版GitHubの基盤ファイル | Chapter 8 | Push後にGitHub上で基盤ファイルの反映を確認する | 必須 | 新しいPrivateテスト用リポジトリ | GitHubユーザー名、URL、他タブ | リポジトリ名の公開可否を事前決定し、不要部分を切り抜く | Public版完成。`Images/S006_foundation_files_github_public.png`をMarkdown参照済み。`00_Command_Center`は閉じた状態である。 |
| S-007 | README.mdだけがChangesにある状態 | Chapter 10 | 第1Commit後、READMEだけを第2Commitの対象にする | 必須 | 新しいPrivateテスト用リポジトリ | README内容、リポジトリ名 | Changes一覧を中心に切り抜く | Public版完成。`Images/S007_readme_changes_public.png`をMarkdown参照済み。 |
| S-008 | README用Summary入力欄 | Chapter 10 | 第2Commit前にSummaryとREADMEだけを確認する | 中 | 新しいPrivateテスト用リポジトリ | README内容、リポジトリ名 | S-007と同じ画面で十分なら別画像にしない | 不採用 |
| S-009 | ブラウザ版GitHubのREADME表示 | Chapter 10、11 | 第2Push後にREADMEを読めることと再開場所を確認する | 必須 | 新しいPrivateテスト用リポジトリ | GitHubユーザー名、URL | READMEとファイル一覧に必要な部分だけを残す | Public版完成。`Images/S009_readme_github_public.png`をMarkdown参照済み。 |
| S-010 | Commit履歴が3件ある状態 | Chapter 10 | Initial、基盤、READMEを分けた結果を確認する | 必須 | 新しいPrivateテスト用リポジトリ | GitHubユーザー名、URL | Commit一覧だけを切り抜く | Public版完成。`S010_commit_history_raw_v3.png`由来の`Images/S010_commit_history_public.png`をMarkdown参照済み。 |
| S-011 | 空フォルダのローカル表示 | Chapter 4、Trouble 2 | ローカルには存在してもGitHubに表示されない場合がある | 中 | 新しいPrivateテスト用リポジトリ | Windowsユーザー名、ローカルパス | 安全なテスト用パスで、フォルダ名だけが読めるようにする | 再現可否確認中 |
| S-012 | GitHub側で空フォルダが見えない状態 | Trouble 2 | 空フォルダが追跡されないことと、作成失敗ではないこと | 中 | 新しいPrivateテスト用リポジトリ | GitHubユーザー名、URL | S-011との比較に必要な部分だけを残す | 再現可否確認中 |
| S-013 | 別リポジトリを開いている例 | Trouble 3 | リポジトリ取り違えの危険 | 低 | 安全に実在する失敗例を再現できる場合のみ | 他リポジトリ名、ローカルパス | 架空のエラー画面を作らず、実在の安全なテスト例だけを使う | 再現可否確認中 |

## 4. 最小撮影セットの実施結果

Version 0.2の最小セットは、次の**8枚**を撮影・加工し、教材用Public画像として`05_Products/Codex_AI_Team_Starter_Kit/Images/`へ配置した。

1. S-001：Current repository
2. S-003：基盤3文書だけのChanges
3. S-004：Summary入力欄とChanges
4. S-005：Push origin
5. S-006：ブラウザ版GitHubの基盤3文書
6. S-007：README.mdだけのChanges
7. S-009：ブラウザ版GitHubのREADME表示
8. S-010：Commit履歴

S-008はS-007またはS-010のキャプションで補えるため、別画像にしない。

## 5. トラブル用画面

通常フローを撮影した後に、次を評価する。

| 候補 | 判定 | 理由 |
| --- | --- | --- |
| 空フォルダ比較（S-011、S-012） | 追加検証後に採用判断 | 実際に確認済みだが、WindowsパスとGitHub情報を安全に伏せられるか確認が必要。 |
| 別リポジトリ選択（S-013） | 追加検証が必要 | 架空の失敗画面にせず、安全なテスト環境で実在の状態を再現できる場合だけ撮影する。 |
| Changesに4ファイルがある状態 | 追加検証が必要 | 実体験は確認済みだが、正常フローの撮影後に安全なテスト環境で再現する。 |
| MARKET_RESEARCH.mdがGitHub側にない状態 | 不採用 | 当時の原因が未確定で、画面だけでは安全な対処を断定できない。 |
| SummaryとCommit内容が一致しない状態 | 不採用 | 具体的な原因と安全な再現方法が未確認。 |

## 6. 撮影順序（実施済み）

1. 新しいPrivateテスト用リポジトリを準備する。
2. S-001：Current repositoryを撮影する。
3. 基盤3文書を作成し、S-003とS-004を撮影する。
4. 人間が第1Commit後、S-005を撮影する。
5. Push後、S-006を撮影する。
6. CodexへREADME.md一件だけを依頼する。
7. README作成後、S-007を撮影する。
8. 人間が第2Commit・Pushを行った後、S-009とS-010を撮影する。

撮影のために本番リポジトリを変更しない。

## 7. 撮影環境

撮影環境は、次の一つに固定する。

- 新しいPrivateテスト用リポジトリ
- Windows
- GitHub Desktop
- ブラウザ版GitHub
- Codex
- 個人情報を含まない架空のプロジェクト名
- 個人情報・認証情報を含まないテスト用ファイル内容

本番の`AI Automation Project`を撮影元にしない。

## 8. 個人情報保護ルール

- 本名、メールアドレス、Windowsのユーザーフォルダ名を写さない。
- GitHubユーザー名、リポジトリURL、ローカルパスは公開可否を撮影前に判断する。
- 通知、ブラウザタブ、ブックマーク、他のリポジトリ名、個人用ファイル名を撮影前に除く。
- APIキー、アクセストークン、認証情報は写さない。
- 後からぼかすより、撮影前に安全なテスト環境を作ることを優先する。
- 隠す場合は、隠した箇所から元の情報を推測できない状態にする。

## 9. 加工ルール

- 必要箇所だけを切り抜く。
- 矢印や枠は最小限にし、1画面で伝える操作対象は一つに絞る。
- UIを改変して見せず、架空の成功・失敗画面を合成しない。
- 元画像を公開用フォルダへ直接置かない。
- 加工前（raw）と教材掲載用（public）を分けて管理する。

## 10. ファイル命名規則

形式は次を使う。

```text
S001_current_repository_raw.png
S001_current_repository_public.png
```

- `raw`：非公開原本
- `public`：教材掲載用
- 番号：この計画のIDと一致させる

## 11. 保存先と記録用原本

教材に掲載するPublic画像は、次の場所へ配置済みである。

```text
05_Products/
└── Codex_AI_Team_Starter_Kit/
    └── Images/
        ├── S001_current_repository_public.png
        ├── S003_foundation_changes_public.png
        ├── S004_summary_and_changes_public.png
        ├── S005_push_origin_public.png
        ├── S006_foundation_files_github_public.png
        ├── S007_readme_changes_public.png
        ├── S009_readme_github_public.png
        └── S010_commit_history_public.png
```

- Raw画像はリポジトリ外の記録用原本として保持し、Gitへ追加しない。
- 旧`S010_commit_history_raw.png`は失敗例、`S010_commit_history_raw_v2.png`は途中確認記録として保持する。どちらも正常フロー用Public画像には使用しない。
- 正常フロー用のS-010 Public画像は、`S010_commit_history_raw_v3.png`を元に作成したものだけを使用する。
- `.gitignore`は今回変更しない。

## 12. 画面ごとの完了条件

各画面は、次をすべて満たした場合だけ教材掲載候補とする。

- 伝えたい情報が一つに絞られている。
- 文字が読める。
- 不要な情報が写っていない。
- 個人情報・認証情報がない。
- 使用章が決まっている。
- UIの状態が実際の操作と一致する。
- キャプション候補がある。

## 13. 撮影チェックリスト

- [ ] テスト用Privateリポジトリを使用した。
- [ ] 本番リポジトリを使用していない。
- [ ] 個人情報を含まないプロジェクト名を使用した。
- [ ] 不要なブラウザタブを閉じた。
- [ ] 通知を隠した。
- [ ] ローカルパスに個人名が出ていないか確認した。
- [ ] GitHubユーザー名の扱いを確認した。
- [ ] 画面ごとに伝える内容を一つに絞った。
- [ ] raw画像とpublic画像を分けた。
- [ ] public画像を拡大して再確認した。
- [ ] UIを偽造していない。
- [ ] 撮影日とアプリバージョンを記録した。

## 14. 完了条件

- [x] Version 0.2の最小8枚が確定している。
- [x] 各画面の使用章が決まっている。
- [x] 撮影順序を実施した。
- [x] 個人情報保護方針がある。
- [x] rawとpublicの管理方針がある。
- [x] 未確認の失敗画面を無理に採用していない。
- [x] 本番環境を変更せず撮影した。
