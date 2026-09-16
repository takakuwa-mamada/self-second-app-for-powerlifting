B·I·L — ローンチ用パッケージ

【中身】
  index.html        アプリ本体
  manifest.json     PWA設定（アプリ名・アイコン・テーマ色）
  sw.js             サービスワーカー（オフライン動作）
  icons/            アプリアイコン一式（192/512/maskable/apple-touch/favicon/1024）

【Web公開（最短・数分）】
  このフォルダごとを静的ホスティングに置くだけ:
  - Cloudflare Pages / Netlify / GitHub Pages いずれも可
  - HTTPSで配信されればサービスワーカー（オフライン）とインストールが有効化
  - スマホで開き「ホーム画面に追加」で通常アプリのように起動

【アプリストアに出す（PWABuilder経由）】
  1. 上記でWeb公開しHTTPSのURLを用意
  2. PWABuilder.com にURLを入力 → Android(.aab) / iOS パッケージを生成
  3. Google Play: 登録料 約$25(一度きり)。2023/11以降作成の個人アカウントは
     本番公開前に「12人・14日間のクローズドテスト」が必要（部の仲間で充足可）
  4. App Store: Apple Developer Program 約$99/年。審査あり
  5. どちらもプライバシーポリシーのURLが必要（データは端末内保存＝収集なしと明記可）

  icons/icon-1024.png はストア掲載用アイコンに使えます。
