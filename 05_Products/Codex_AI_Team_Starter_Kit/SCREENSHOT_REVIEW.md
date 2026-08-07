# SCREENSHOT REVIEW

## 1. レビュー概要

- **レビュー対象**：最小スクリーンショット8枚（Raw画像）
- **レビュー目的**：初心者向け教材へ掲載する前に、画面状態・可読性・識別情報・本文との対応を確認し、採用方針を決める。
- **レビュー日**：2026-08-06
- **Raw画像の保存場所**：`C:\Users\spiri\Documents\Codex\2026-08-01\Assets\Codex_Starter_Kit\Raw`
- **Public画像の保存予定場所**：`C:\Users\spiri\Documents\Codex\2026-08-01\Assets\Codex_Starter_Kit\Public`（今回の作成・移動は未実施）
- **今回未実施**：画像加工、撮り直し、Raw画像の移動、教材本文への挿入、Gitへの画像追加、Commit、Push。

判定は、正常フローの説明画像と、実際の失敗例として価値がある画像を混同しないことを優先した。

## 2. 画像別レビュー

| ID | 使用章 | 判定 | 良い点 | 問題点 | 必要な加工 | 撮り直し要否 | Publicファイル名 |
|---|---|---|---|---|---|---|---|
| S-001 | Chapter 03 | 採用 | `Current repository`、対象リポジトリ、`main`、Changesが空の初期状態を一画面で確認できる。 | リポジトリ名は末尾が省略表示されている。 | 上部のCurrent repositoryと`main`が読みやすい範囲へ軽く切り抜く。 | 不要 | `S001_current_repository_public.png` |
| S-003 | Chapter 08 | 条件付き採用 | Changesに基盤3文書だけがあることを明確に示せる。 | 黄色の改行コード通知は本章の目的と無関係で、初心者の注意を散らす。 | Changes一覧と3ファイルが読める範囲を残し、通知バーは切り抜く。 | 不要 | `S003_foundation_changes_public.png` |
| S-004 | Chapter 08 | 条件付き採用 | SummaryとChangesの3ファイルを同時に照合できる。 | 改行コード通知があり、画面下部に余白が多い。 | 通知バーと不要な余白を切り抜き、Summary欄とChanges一覧だけを残す。 | 不要 | `S004_summary_and_changes_public.png` |
| S-005 | Chapter 08 | 条件付き採用 | Commit後にChangesが空となり、`Push origin`が表示される状態を明確に示す。 | 画面下部に、重複した基盤Commitメッセージの一部が見える。 | 下部のCommitメッセージ表示を切り抜き、`Push origin`と`No local changes`を残す。 | 不要 | `S005_push_origin_public.png` |
| S-006 | Chapter 08 | 条件付き採用 | ブラウザ版GitHubで`AGENTS.md`と`00_Command_Center`を確認する流れが分かる。 | GitHubユーザー名、Commitハッシュ、重複したCommitメッセージが見える。正常例のCommitメッセージとしては使えない。 | ユーザー名をぼかす。Commitメッセージ・ハッシュ欄を切り抜くか隠し、ファイル一覧だけを使う。 | 不要（ファイル反映確認に限定する場合） | `S006_foundation_files_github_public.png` |
| S-007 | Chapter 10 | 条件付き採用 | Changesに`README.md`だけが表示される再テスト成功を明確に示す。 | Summary欄の`Create README.md`は本文で推奨するSummaryと異なるため、同時に見せると混乱する。 | Changes一覧と`README.md`だけが見える範囲へ切り抜き、Summary欄を除く。 | 不要 | `S007_readme_changes_public.png` |
| S-009 | Chapter 10 | 条件付き採用 | ブラウザ版GitHubでREADME本文とルート直下の`README.md`を確認する画面として有用。 | GitHubユーザー名、Commitハッシュ、リポジトリ名が表示される。 | ユーザー名とCommitハッシュをぼかす。必要に応じてリポジトリ名も汎用名へぼかす。 | 不要 | `S009_readme_github_public.png` |
| S-010 v3 | Chapter 10（補助） | 条件付き採用 | Commits一覧に、`docs: プロジェクトREADMEを追加`、`docs: プロジェクト基盤を追加`、`Initial commit`の3件が時系列で表示される。Commitメッセージの重複はない。 | GitHubユーザー名、Commitハッシュ、日付・時刻、テスト用リポジトリ名が表示される。 | ユーザー名・Commitハッシュをぼかし、必要に応じてリポジトリ名をぼかす。Commits一覧と3件のメッセージは残す。 | 不要 | `S010_commit_history_public.png` |

## 3. 個人情報・識別情報

| 画像 | 識別情報 | 判定 | 方針 |
|---|---|---|---|
| S-001 | テスト用リポジトリ名、GitHub DesktopのUI、取得時刻表示 | 公開可能 | リポジトリ名はテスト用であり、個人名・ローカルパスは見えない。必要に応じて上部だけを切り抜く。 |
| S-003 | テスト用リポジトリ名、GitHub DesktopのUI | 公開可能 | ローカルパス・Windowsユーザー名・認証情報は見えない。黄色の通知は切り抜く。 |
| S-004 | テスト用リポジトリ名、GitHub DesktopのUI | 公開可能 | ローカルパス・Windowsユーザー名・認証情報は見えない。通知と余白を切り抜く。 |
| S-005 | テスト用リポジトリ名、Commitメッセージ断片、GitHub DesktopのUI | 切り抜く | Commitメッセージ断片は正常例に不要なため切り抜く。 |
| S-006 | GitHubユーザー名、テスト用リポジトリ名、Commitハッシュ、Commitメッセージ、ブラウザUI | 隠す | ユーザー名・ハッシュをぼかす。重複メッセージを含む欄は切り抜く。 |
| S-007 | テスト用リポジトリ名、Summary入力内容、GitHub DesktopのUI | 切り抜く | Summary欄を除き、READMEだけがChangesにある部分を使う。 |
| S-009 | GitHubユーザー名、テスト用リポジトリ名、Commitハッシュ、ブラウザUI | 隠す | ユーザー名・ハッシュをぼかす。テスト用リポジトリ名は公開用の表現方針に合わせて必要ならぼかす。 |
| S-010（旧） | GitHubユーザー名、Commitハッシュ、日付・時刻、ブラウザUI、重複Commitメッセージ | 隠す | 正常フロー用には使用しない。失敗例へ転用する場合のみ、ユーザー名・ハッシュをぼかす。 |
| S-010 v2 | GitHubユーザー名、テスト用リポジトリ名、Commitハッシュ、日付・時刻、ブラウザUI | 隠す | 正常なCommitメッセージは確認できるが、画面種別が要件と異なる。Commits一覧を撮影し直す場合も、ユーザー名・ハッシュをぼかす。 |
| S-010 v3 | GitHubユーザー名、テスト用リポジトリ名、Commitハッシュ、日付・時刻、ブラウザUI | 隠す | 正常フロー用の採用候補。ユーザー名・ハッシュをぼかし、Commits一覧と3件のメッセージを残す。 |

8枚すべてで、Windowsユーザー名、ローカルパス、メールアドレス、APIキー、アクセストークン、他のブラウザタブ、通知、ブックマークは確認できなかった。

## 4. 最小加工方針

| ID | Public版で行う最小加工 |
|---|---|
| S-001 | 余白を切り抜く。Current repositoryと`main`を一つの枠で示す。 |
| S-003 | 黄色の通知バーを切り抜く。Changesの3ファイルだけを一つの枠で示す。 |
| S-004 | 黄色の通知バーと余白を切り抜く。Summary欄とChanges一覧を一つの枠で示す。 |
| S-005 | 画面下部のCommitメッセージを切り抜く。`Push origin`を一つの枠で示す。 |
| S-006 | ユーザー名をぼかし、Commitメッセージ・ハッシュ欄を切り抜く。ファイル一覧を一つの枠で示す。 |
| S-007 | Summary欄を切り抜く。Changesの`README.md`だけを一つの枠で示す。 |
| S-009 | ユーザー名とCommitハッシュをぼかす。`README.md`の本文とファイルツリーを一つの枠で示す。 |
| S-010（旧） | 正常フロー用のPublic版は作成しない。失敗例として転用する場合のみ、ユーザー名・ハッシュをぼかし、重複メッセージに「Summaryと対象ファイルをCommit前に照合する」の注釈を一つ付ける。 |
| S-010 v2 | Public版は作成しない。途中確認記録としてRaw画像を保持する。 |
| S-010 v3 | ユーザー名・Commitハッシュをぼかす。必要に応じてリポジトリ名をぼかす。Commits一覧と3件のメッセージを残し、枠や矢印は追加しない。 |

矢印や枠は、各画像につき一つに限定する。説明はキャプションで補い、画面上へ文章を増やしすぎない。

## 5. 撮り直し候補

### S-010 v3：Commit履歴の正常フロー用

- **Raw画像**：`S010_commit_history_raw_v3.png`
- **確認できた事実**：ブラウザ版GitHubのCommits一覧に、`docs: プロジェクトREADMEを追加`、`docs: プロジェクト基盤を追加`、`Initial commit`の3件が上から順に表示されている。Commitメッセージの重複はない。
- **正常フローでの扱い**：Chapter 10の補助画像として条件付き採用する。第1Commitと第2Commitが別々に残ることを示す。
- **Public版の条件**：ユーザー名・Commitハッシュをぼかす。Commits一覧、3件のCommitメッセージ、`main`は残す。

### S-010 v2：途中確認記録

- **Raw画像**：`S010_commit_history_raw_v2.png`
- **扱い**：削除・上書きはしない。Commitメッセージが正常であることを確認した途中記録としてRawフォルダに保持する。
- **教材への掲載**：Commits一覧ではないため、正常フロー・失敗例のどちらにも掲載しない。

### S-010（旧）：実際の失敗例

- **Raw画像**：`S010_commit_history_raw.png`
- **扱い**：正常フローには使用しない。削除・上書きも行わない。
- **転用先**：`Trouble-T-006`に関連する、Commitメッセージの重複を示す実際の失敗例。
- **Public版を作る場合**：GitHubユーザー名・Commitハッシュをぼかし、「SummaryとChangesをCommit前に照合する」という注釈を一つだけ加える。

既存のテスト用リポジトリの履歴は書き換えない。正常例を作る必要がある場合は、新しいテスト用リポジトリで再現する。

## 6. 本文との対応

| 画像ID | 使用章 | 挿入候補位置 | 画像で補う内容 | 本文だけでは不足する理由 |
|---|---|---|---|---|
| S-001 | Chapter 03 | Current repositoryを確認する手順の直後 | 画面左上のCurrent repositoryと`main` | 初心者は確認箇所を画面上で見つけにくい。 |
| S-003 | Chapter 08 | 第1Commit前のChanges確認 | 基盤3文書だけが並ぶ状態 | 「3ファイルだけ」の判定を視覚的に照合できる。 |
| S-004 | Chapter 08 | Summary入力前の確認 | SummaryとChangesを照合する位置 | 何を一致させるのかを一画面で示せる。 |
| S-005 | Chapter 08 | Commit後、Push前の手順 | `Push origin`とChangesが空の状態 | Commit後に何が変わるかを確認できる。 |
| S-006 | Chapter 08 | Push後のブラウザ版GitHub確認 | 基盤3文書がGitHub上にあること | ローカル確認とブラウザ確認の違いを示せる。 |
| S-007 | Chapter 10 | 第2Commit前のChanges確認 | `README.md`だけがある状態 | 第1Commitと第2Commitを分ける理由を視覚化できる。 |
| S-009 | Chapter 10 | Push後のREADME確認 | GitHub上のREADME本文とファイルツリー | Push後にブラウザ版で確認する終点を示せる。 |
| S-010 v3 | Chapter 10（補助） | 2段階Commitの確認補助 | Commit履歴の分離 | 第1Commitと第2Commitが別々に残ることを確認できる。 |

## 7. トラブル集へ転用する画像

- **S-006**：重複メッセージが写る部分は、正常フローには使わない。切り抜かずに使う場合は、Commitメッセージの確認不足を示す補助的な失敗例に限定する。
- **S-010（旧）**：正常フロー用には不採用とし、`Trouble-T-006`（Summaryと実際の対象ファイルの不一致）に関連する実際の失敗例としては価値がある。転用時は「重複した文字列のCommitメッセージ」という事実だけを説明し、ユーザー名・ハッシュを隠す。
- **S-010 v2**：Commitメッセージの重複がないため、失敗例には使わない。保存画面がCommits一覧ではないため、正常フローにも使わず、途中確認記録としてのみ保持する。
- **S-010 v3**：正常フロー用として条件付き採用する。失敗例には使わない。

## 8. Public版作成順序

1. S-001：正しいリポジトリを確認する入口
2. S-003：基盤3文書だけのChanges
3. S-004：SummaryとChangesの照合
4. S-005：Push origin
5. S-006：GitHub上の基盤3文書
6. S-007：READMEだけのChanges
7. S-009：GitHub上のREADME
8. S-010：`S010_commit_history_raw_v3.png`から、ユーザー名・Commitハッシュを隠して作成。旧S-010とv2はPublic版の正常フローへ使わない。

## 9. 完了チェックリスト

- [x] 8枚すべてを確認した
- [x] 使用章と画像内容を照合した
- [x] 個人情報・識別情報を確認した
- [x] 撮り直し要否を決めた
- [x] S-006とS-010を個別に評価した
- [x] Publicファイル名を決めた
- [x] 加工を増やしすぎていない
- [x] 正常例と失敗例を混同していない
- [x] 既存ファイルを変更していない
- [x] 画像加工を実施していない

## Review Conclusion

S-001、S-003、S-004、S-005、S-006、S-007、S-009、`S010_commit_history_raw_v3.png`は、上記の最小加工を条件に正常フローの教材へ使用できる。旧`S010_commit_history_raw.png`は失敗例としてのみ転用候補とし、`S010_commit_history_raw_v2.png`は途中確認記録としてのみ保持する。
