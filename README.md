# V CUP 2026 大会ホームページ

主催：ヴァリエンテ富山ジュニア

## ファイル構成
- index.html：トップページ（U8/U9選択）
- vcup2026_u8.html：U8カテゴリーページ
- vcup2026_u9.html：U9カテゴリーページ

## GitHub Pagesでの公開手順
1. GitHubにログインする（https://github.com）
2. 右上の「+」→「New repository」をクリック
3. Repository nameに「vcup2026」と入力
4. 「Public」を選択
5. 「Create repository」をクリック
6. 「uploading an existing file」をクリック
7. output/フォルダ内の以下4ファイルをドラッグ＆ドロップ：
   - index.html
   - vcup2026_u8.html
   - vcup2026_u9.html
   - README.md
8. 「Commit changes」をクリック
9. 「Settings」タブ→左メニュー「Pages」をクリック
10. 「Branch」を「main」に変更して「Save」
11. 数分後にURLが発行される
    例：https://（ユーザー名）.github.io/vcup2026/

## Googleスプレッドシート連携の設定方法
1. Googleスプレッドシートを新規作成
2. シート名を以下の通りに設定：
   - U8_A（グループA）
   - U8_B（グループB）
   - U8_C（グループC）
   - U8_D（グループD）
   - U9（U9全体）
3. 各シートの1行目に以下のヘッダーを入力：
   チーム名 / 試合数 / 勝 / 分 / 負 / 得点 / 失点 / 得失点差 / 勝点
4. スプレッドシートの「共有」→「リンクを知っている全員が閲覧可能」に設定
5. URLのIDをコピー（https://docs.google.com/spreadsheets/d/【ここ】/edit）
6. vcup2026_u8.htmlとvcup2026_u9.html内の
   SPREADSHEET_ID という定数に貼り付ける
7. ファイルをGitHubに再アップロードすると順位表が自動更新される

## 当日のスコア入力方法（担当コーチ向け）
1. スマホにGoogleスプレッドシートアプリをインストール
2. 共有されたスプレッドシートURLを開く
3. 試合終了後、該当チームの行を更新する
4. 保存すると30秒以内にホームページの順位表に反映される
