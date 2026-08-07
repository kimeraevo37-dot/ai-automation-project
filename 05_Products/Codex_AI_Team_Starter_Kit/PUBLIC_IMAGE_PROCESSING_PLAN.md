# PUBLIC IMAGE PROCESSING PLAN

## 1. 目的

Raw画像8枚から、初心者向け教材に掲載するPublic画像を安全かつ最小限の加工で作成するための手順書です。

- **Raw保存場所**：`C:\Users\spiri\Documents\Codex\2026-08-01\Assets\Codex_Starter_Kit\Raw`
- **Public保存予定場所**：`C:\Users\spiri\Documents\Codex\2026-08-01\Assets\Codex_Starter_Kit\Public`
- **対象**：正常フロー用の8枚だけ
- **今回の範囲外**：画像加工、Raw画像の変更・移動、Public画像の作成、教材本文変更、Gitへの画像追加、Commit、Push

## 2. 共通加工ルール

1. Raw画像は変更せず、Public版は別ファイルとして作成する。
2. 画面の意味を変えない。UI、Commitメッセージ、ファイル名、状態を画像編集で書き換えない。
3. 必要のない領域は、ぼかすより先に切り抜く。残したい画面情報だけを小さく整える。
4. 個人を識別できるGitHubユーザー名、Commitハッシュ、URL、ローカルパスは、残す必要がなければ切り抜き、残る場合はぼかす。
5. 枠は各画像につき最大1つ、矢印は必要な場合だけ最大1つにする。枠と矢印を同時に増やさない。
6. 説明は短いキャプションで補い、画像の上に長文を追加しない。
7. 切り抜き後も、読者が「どのアプリの、どの状態か」を判断できる見出しまたは必要なUIを残す。

## 3. 画像別加工指示

| ID | Raw | Public | 使用章 | 切り抜き | ぼかし | 枠/矢印 | キャプション |
|---|---|---|---|---|---|---|---|
| S-001 | `S001_current_repository_raw.png` | `S001_current_repository_public.png` | Chapter 03 | Current repository、対象リポジトリ名、`main`、Changesが空の状態を残す。不要な下部余白を除く。 | なし。リポジトリ名を公開しない方針の場合だけぼかす。 | Current repositoryと`main`を囲む枠1つ。矢印なし。 | 「作業前に、Current repositoryとmainを確認します。」 |
| S-003 | `S003_foundation_changes_raw.png` | `S003_foundation_changes_public.png` | Chapter 08 | Changes一覧と3ファイルを残す。LF/CRLFの黄色い通知バー、不要な右側・下側の余白を除く。 | なし。 | Changesの3ファイル一覧を囲む枠1つ。矢印なし。 | 「第1Commitの前に、基盤3文書だけがChangesにあることを確認します。」 |
| S-004 | `S004_summary_and_changes_raw.png` | `S004_summary_and_changes_public.png` | Chapter 08 | Summary欄と3ファイルのChanges一覧を残す。LF/CRLFの黄色い通知バーと不要な余白を除く。 | なし。 | Summary欄とChanges一覧をまとめて囲む枠1つ。矢印なし。 | 「SummaryとChangesの対象が一致していることを確認します。」 |
| S-005 | `S005_push_origin_raw.png` | `S005_push_origin_public.png` | Chapter 08 | `Push origin`、Changesが空、Commit後の状態が分かる部分を残す。下部の不要なCommitメッセージ表示を除く。 | なし。 | `Push origin`を囲む枠1つ。矢印なし。 | 「Commit後、Push originが表示されたことを確認します。」 |
| S-006 | `S006_foundation_files_github_raw.png` | `S006_foundation_files_github_public.png` | Chapter 08 | GitHub上の`AGENTS.md`と`00_Command_Center`の一覧を残す。Commitメッセージ欄、ハッシュ欄、不要な右側情報を除く。 | GitHubユーザー名。残るCommitハッシュ。必要に応じてテスト用リポジトリ名。 | ファイル一覧を囲む枠1つ。矢印なし。 | 「Push後、ブラウザ版GitHubで基盤3文書の反映を確認します。」 |
| S-007 | `S007_readme_changes_raw.png` | `S007_readme_changes_public.png` | Chapter 10 | Changesの`README.md`だけと「1 changed file」が分かる部分を残す。Summary欄、通知バー、不要な差分本文を除く。 | なし。 | `README.md`を囲む枠1つ。矢印なし。 | 「第2Commitの前に、README.mdだけがChangesにあることを確認します。」 |
| S-009 | `S009_readme_github_raw.png` | `S009_readme_github_public.png` | Chapter 10 | README本文の見出し、`README.md`が選択されたファイルツリーを残す。不要な上部・右側UIを除く。 | GitHubユーザー名、Commitハッシュ。必要に応じてテスト用リポジトリ名。 | README本文またはファイルツリーのどちらか一方を囲む枠1つ。矢印なし。 | 「Push後、ブラウザ版GitHubでREADME.mdを確認します。」 |
| S-010 | `S010_commit_history_raw_v3.png` | `S010_commit_history_public.png` | Chapter 10（補助） | `main`、Commits一覧、3件のCommitメッセージを残す。不要な上部ナビゲーションと余白を除く。 | GitHubユーザー名、3件のCommitハッシュ。必要に応じてテスト用リポジトリ名。 | 枠・矢印なし。3件の履歴がそのまま読める構図を優先する。 | 「基盤3文書とREADME.mdが別々のCommitとして履歴に残ります。」 |

### S-001：Current repository

- **画像の役割**：正しいリポジトリを開いていることを確認する入口。
- **残す範囲**：画面左上のCurrent repository、対象リポジトリ名、Current branchの`main`、Changesが空の表示。
- **加工後の確認**：リポジトリ名が読めるか、他のリポジトリ名・ローカルパス・ユーザー名が写っていないか。

### S-003：基盤3文書のChanges

- **画像の役割**：第1Commitの対象を3ファイルへ絞る確認。
- **残す範囲**：Changesの件数と、`AGENTS.md`、`ROADMAP.md`、`COMPANY_RULE.md`が並ぶ一覧。
- **加工後の確認**：黄色いLF/CRLF通知バーが除外され、README.mdや他ファイルが表示されていないか。

### S-004：SummaryとChanges

- **画像の役割**：Commit前にSummaryと対象ファイルを照合する確認。
- **残す範囲**：入力済みSummaryと基盤3文書のChanges一覧。
- **加工後の確認**：Summaryが一度だけ表示され、3ファイルとの関係が読み取れるか。LF/CRLF通知を残していないか。

### S-005：Push origin

- **画像の役割**：Commit後、Push前の状態を示す。
- **残す範囲**：`Push origin`、Changesが空であること、Commit済みであることが分かる部分。
- **加工後の確認**：重複したCommitメッセージや不要な履歴断片を残していないか。`Push origin`が読み取れるか。

### S-006：GitHub上の基盤3文書

- **画像の役割**：Push後、ブラウザ版GitHubでファイル反映を確認する。
- **残す範囲**：GitHubのファイル一覧で、`AGENTS.md`と`00_Command_Center`を確認できる部分。
- **加工後の確認**：ユーザー名・ハッシュを隠したうえで、Commitメッセージ欄が主役になっていないか。基盤ファイルの反映が読めるか。

### S-007：READMEだけのChanges

- **画像の役割**：READMEを第2Commitへ分ける確認。
- **残す範囲**：Changesに`README.md`だけが表示される部分。
- **加工後の確認**：Summary欄、不要な差分本文、黄色い通知バーを残していないか。`README.md`だけであることが明確か。

### S-009：GitHub上のREADME

- **画像の役割**：READMEがPush後にブラウザ版GitHubへ反映された終点を示す。
- **残す範囲**：README本文の見出しと、ルート直下の`README.md`が選択されているファイルツリー。
- **加工後の確認**：ユーザー名・ハッシュをぼかしたか。README本文を不自然に切り抜いて意味を変えていないか。

### S-010：正常なCommit履歴

- **画像の役割**：第1Commitと第2Commitが分かれていることを補助的に確認する。
- **使用するRaw画像**：`S010_commit_history_raw_v3.png`のみ。
- **残す範囲**：`main`と、次の3件のCommitメッセージ。
  - `docs: プロジェクトREADMEを追加`
  - `docs: プロジェクト基盤を追加`
  - `Initial commit`
- **除外するRaw画像**：`S010_commit_history_raw.png`（失敗例）、`S010_commit_history_raw_v2.png`（途中確認記録）。
- **加工後の確認**：3件の順番を変えていないか。ユーザー名・ハッシュが見えないか。Commitメッセージを加工で書き換えていないか。

## 4. 個人情報保護チェック

Public画像の作成前と作成後に、次を画像ごとに確認する。

- [ ] GitHubユーザー名を切り抜きまたはぼかした
- [ ] Commitハッシュを切り抜きまたはぼかした
- [ ] URL、ローカルパス、Windowsユーザー名が写っていない
- [ ] メールアドレス、通知、他のブラウザタブ、ブックマークが写っていない
- [ ] APIキー、アクセストークン、パスワードが写っていない
- [ ] テスト用リポジトリ名を公開してよいか確認した

## 5. 加工後の品質チェック

- [ ] 文字が読める大きさを維持した
- [ ] 画面の状態を誤解させる切り抜きをしていない
- [ ] 正常フローと失敗例を混同していない
- [ ] 枠は1つ以下、矢印は必要な場合だけ1つ以下にした
- [ ] 黄色いLF/CRLF通知をS-003・S-004へ残していない
- [ ] S-005に不要なCommitメッセージを残していない
- [ ] S-006で基盤3文書の反映が主役になっている
- [ ] S-007でREADME.mdだけがChangesにあることが分かる
- [ ] S-010で3件のCommitメッセージと`main`が読める
- [ ] Public版のファイル名が指定どおりである

## 6. Public画像作成順序

1. `S001_current_repository_public.png`
2. `S003_foundation_changes_public.png`
3. `S004_summary_and_changes_public.png`
4. `S005_push_origin_public.png`
5. `S006_foundation_files_github_public.png`
6. `S007_readme_changes_public.png`
7. `S009_readme_github_public.png`
8. `S010_commit_history_public.png`

## 7. 完了チェックリスト

- [ ] 8枚すべてに加工指示がある
- [ ] Rawファイル名とPublicファイル名が対応している
- [ ] S-010はv3を使用している
- [ ] ユーザー名の処理方針がある
- [ ] Commitハッシュの処理方針がある
- [ ] LF/CRLF通知の処理方針がある
- [ ] 正常フローの意味を壊す加工がない
- [ ] 加工を増やしすぎていない
- [ ] 教材本文との対応が分かる
- [ ] 実際の画像加工は行っていない
