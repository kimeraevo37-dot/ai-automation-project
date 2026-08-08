# 購入者向け配布パッケージ構成計画

## 1. 目的

購入者が最初に開くファイル、教材本文、テンプレート、困ったときの参照先を迷わず見つけられる配布パッケージを設計する。これは配布構成の計画であり、現時点でファイル移動、コピー、ZIP作成、PDF作成は行わない。

## 2. 購入者へ渡すもの

- `START_HERE.md`（配布時に新規作成する開始案内）
- `Course/` 内の Chapter 00〜11
- `Images/` 内の正常フロー用Public画像8枚
- `Templates/` 内の購入者向けテンプレート
  - `AGENTS_TEMPLATE.md`
  - `COMPANY_RULE_TEMPLATE.md`
  - `ROADMAP_TEMPLATE.md`
  - `FOLDER_STRUCTURE.md`
  - `FIRST_TASK_PROMPT.md`
  - `CHANGELOG.md`（購入者のプロジェクトで使うテンプレート）
- `Appendix/` にまとめた4付録
  - `COMMIT_CHECKLIST.md`
  - `GLOSSARY.md`
  - `TROUBLESHOOTING.md`
  - `FAQ.md`
- 配布物自身の更新履歴としての `CHANGELOG.md`（配布時に新規作成する）

## 3. 購入者へ渡さないもの

次は開発、検証、運用のための資料であり、通常の購入者向け配布物には含めない。

- `PRODUCT_REQUIREMENTS.md`、`COURSE_OUTLINE.md`、`CONTENT_SOURCE_SELECTION.md`
- `VERSION_0_2_PLAN.md`、`APPENDIX_PLAN.md`
- `SCREENSHOT_PLAN.md`、`SCREENSHOT_REVIEW.md`、`PUBLIC_IMAGE_PROCESSING_PLAN.md`
- `THIRD_PARTY_TEST_PLAN.md`、`THIRD_PARTY_TEST_GUIDE.md`、`TESTER_RECRUITMENT.md`
- 市場調査、意思決定ログ、開発ログ、テスト結果
- Raw画像、失敗例画像、撮影途中の画像
- 本番リポジトリの運営文書、個人情報、認証情報

第三者テストで得た改善内容は、反映後の教材・付録として配布する。内部の記録そのものを無条件には配布しない。

## 4. 推奨フォルダ構成

配布用には、開発用リポジトリとは別の作業場所で次の構成を作る。

```text
Codex_AI_Team_Starter_Kit/
├── START_HERE.md
├── CHANGELOG.md
├── Course/
│   ├── Chapter_00_Getting_Started.md
│   ├── ...
│   └── Chapter_11_Resume_Work.md
├── Templates/
│   ├── AGENTS_TEMPLATE.md
│   ├── COMPANY_RULE_TEMPLATE.md
│   ├── ROADMAP_TEMPLATE.md
│   ├── FOLDER_STRUCTURE.md
│   ├── FIRST_TASK_PROMPT.md
│   └── CHANGELOG.md
├── Images/
│   └── 正常フロー用Public画像8枚
└── Appendix/
    ├── COMMIT_CHECKLIST.md
    ├── GLOSSARY.md
    ├── TROUBLESHOOTING.md
    └── FAQ.md
```

購入者が最初に開くファイルは `START_HERE.md` の一つに固定する。配布物自身の `CHANGELOG.md` と、購入者プロジェクト用の `Templates/CHANGELOG.md` は役割が異なるため、同じ名前でも置き場所を分ける。

## 5. START_HERE.md の役割と構成

`START_HERE.md` は教材の目次を繰り返す文書ではなく、開始地点と戻り先を示す案内にする。本文は配布準備時に作成する。

含める項目は次のとおり。

1. この教材でできること
2. 対象者と、この教材で扱わないこと
3. 必要な環境（GitHub、GitHub Desktop、Codex、テスト用Privateリポジトリ）
4. 最初に読む `Course/Chapter_00_Getting_Started.md`
5. Chapterを順番に進める方法
6. `Templates/` をコピーして使う方法
7. Commit前に見る `Appendix/COMMIT_CHECKLIST.md`
8. 用語、FAQ、想定外の状態への戻り先
9. 配布物の更新履歴である `CHANGELOG.md`
10. サポート範囲はVersion 1.0で確定予定であること

## 6. Course

`Course/` はChapter 00〜11を順番に読む教材本文として、そのまま配布する。画像リンクは現在 `../Images/` を参照しているため、推奨構成でもリンクの階層は変わらない。

本文だけでも手順が成立し、Imagesは確認を補助する役割を維持する。Chapter本文をPDFだけに置き換えることは、この時点では前提にしない。

## 7. Templates

現在の `Templates/` には、購入者向けのテンプレート6件だけがあるため、配布候補として妥当である。

テンプレートは読み取り用の教材本文とは別に置き、購入者が自分のプロジェクトへコピーして使うものとして案内する。`Templates/CHANGELOG.md` は購入者プロジェクトの変更履歴用であり、配布物の更新履歴ではないことを `START_HERE.md` で区別する。

## 8. Images

`Images/` の正常フロー用Public画像8枚は、CourseのMarkdown表示に必要なため配布物へ含める。

- 含める：S001、S003、S004、S005、S006、S007、S009、S010のPublic画像
- 含めない：Raw画像、旧S-010、S-010 v2、失敗例、撮影途中の画像

`Course/` から `../Images/` へのリンクを維持するため、ImagesはCourseと同じ配布ルート直下に置く。

## 9. Appendix

購入者向けには、4付録を `Appendix/` にまとめる案を採用候補とする。困ったときの参照先が一か所にまとまり、教材本文と役割を分けやすいためである。

現在の開発用リポジトリでは4付録は商品ルート直下にある。配布時に4付録をまとめて `Appendix/` へコピーまたは移動する場合、次を確認する。

- `FAQ.md` 内の `Course/` へのリンクは `../Course/` に更新する
- FAQ内の同じAppendix内の付録リンクは、4付録をまとめて移す場合はファイル名だけの参照を維持できる
- `START_HERE.md` からは `Appendix/` を明示して案内する
- Chapterから付録への新規リンクを追加する場合は、配布構成でリンク切れがないか確認する

この変更は配布パッケージ作成時の候補であり、現在のリポジトリの4付録は移動しない。

## 10. CHANGELOG / 更新案内

配布物のルートに置く `CHANGELOG.md` は、教材のVersion、更新日、変更概要、更新時の確認事項を記録する文書にする。これは `Templates/CHANGELOG.md` と別物である。

更新案内は `START_HERE.md` から参照し、購入者が「教材の更新」と「自分のプロジェクトの変更履歴」を混同しないようにする。

## 11. 配布形式4案の比較

| 形式 | 初心者向け | 更新性 | テンプレート利用 | 画像 | 注意点 |
|---|---|---|---|---|---|
| A. フォルダ / ZIP配布 | 解凍後に `START_HERE.md` を開けば始めやすい | 更新版を再配布する必要がある | コピーして使いやすい | フォルダ構成を保てる | 解凍方法とMarkdownを開く方法の案内が必要 |
| B. GitHubリポジトリ配布 | GitHubに不慣れな人には操作が増える | 更新履歴を確認しやすい | ファイル閲覧はしやすいが、コピー手順の案内が必要 | ブラウザで表示しやすい | 公開範囲、ダウンロード方法、GitHubアカウントの扱いを決める必要がある |
| C. PDF + テンプレートZIP | 本文を読むだけなら始めやすい | PDFとZIPを別々に更新する必要がある | テンプレートはZIPから取り出せる | PDF内に埋め込める | 本文とテンプレートが分かれ、リンクや更新の管理が複雑になる |
| D. Markdown + Templates + ImagesのZIP | 現在の教材構成を保てる | 1パッケージ単位で更新できる | 同じフォルダ内でコピーしやすい | 現在の相対リンクを保ちやすい | 購入者のMarkdown閲覧方法を開始案内で明確にする必要がある |

## 12. 推奨配布形式

現時点の仮案は **D. Markdown + Templates + ImagesのZIP** である。現在のCourseとImagesの相対リンクを維持し、教材、テンプレート、付録を一つの配布ルートにまとめられるためである。

この判断は第三者テスト未実施の段階の仮案である。テスターがMarkdownの閲覧やテンプレートの利用で迷うかは、第三者テスト結果を待って確認する。

## 13. 現在のリポジトリから変更が必要な点

実際に配布パッケージを作成する段階では、次を候補として検討する。

- 配布用ルートへ `START_HERE.md` を新規作成する
- 配布物自身の `CHANGELOG.md` を新規作成する
- 4付録を配布用の `Appendix/` に集約する
- Appendix移動に伴うFAQの `Course/` リンクを確認・更新する
- 配布フォルダを別に作り、内部資料を除いた状態でリンクと画像を確認する

開発用リポジトリの構成を、配布構成へ無理に移し替える必要はない。配布物は専用の出力フォルダとして作る。

## 14. Version 1.0前の確定事項

### 必須

- 購入者向けに含めるファイルと内部資料の除外基準
- `START_HERE.md` の本文と開始手順
- 4付録の配布位置とリンク
- Course、Images、Appendix間のリンク確認
- 配布物の更新履歴の運用方法
- 個人情報、認証情報、Raw画像、失敗例が含まれない確認

### 第三者テスト後

- Markdownを読む方法が初心者に分かるか
- `START_HERE.md` の案内だけで開始できるか
- Appendixの置き場所と参照先が分かりやすいか
- PDF併用が必要か
- FAQ、トラブル集、開始案内へ反映する改善点

### 販売サービス決定後

- ZIP、GitHub、ダウンロードページのどれで届けるか
- 更新版の配布方法と購入者への告知方法
- サポート範囲、問い合わせ窓口、返金・利用条件の扱い
- 販売サービスのファイル容量、ダウンロード回数、公開設定への対応

## 15. パッケージ作成時のチェックリスト

- [ ] `START_HERE.md` が配布ルート直下にある
- [ ] CourseのChapter 00〜11が揃っている
- [ ] Imagesに正常フロー用Public画像8枚だけがある
- [ ] CourseからImagesへのリンクがすべて開ける
- [ ] Templatesに購入者向け6ファイルが揃っている
- [ ] Appendixに4付録が揃っている
- [ ] Appendix内とAppendixからCourseへのリンクを確認した
- [ ] Raw画像、失敗例画像、内部計画、テスト資料、市場調査を含めていない
- [ ] 個人情報、認証情報、個人用パス、不要なURLが含まれていない
- [ ] 解凍後の配布ルートだけで教材を読める
- [ ] 更新履歴と配布Versionを確認できる

## 16. 作成順序

1. 第三者テスト結果を確認し、教材・付録・開始案内へ必要な改善を決める。
2. `START_HERE.md` と配布物用 `CHANGELOG.md` の本文を作成する。
3. 専用の配布用フォルダに、購入者向けファイルだけを集める。
4. Course、Images、Appendixのリンクを配布フォルダ内で確認する。
5. 個人情報、認証情報、内部資料、Raw画像がないことを確認する。
6. 選択した販売形式で配布物を作成し、別の場所へ展開して開始手順を確認する。
