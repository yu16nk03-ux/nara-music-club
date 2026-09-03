# NMC LINE Login 設定メモ

今回のZIPでは、SupabaseのPublishable keyを使ってLINEログインを接続しています。

## 使用しているSupabase URL
REST APIのURLではなく、プロジェクトURLを使用します。

https://rxkofbwiejzizpxmhqhq.supabase.co

## Supabase側
- Custom Provider: LINE
- Identifier: custom:line
- Issuer: https://access.line.me
- Authorization URL: https://access.line.me/oauth2/v2.1/authorize
- Token URL: https://api.line.me/oauth2/v2.1/token
- Userinfo URL: https://api.line.me/oauth2/v2.1/userinfo
- JWKS URI: https://api.line.me/oauth2/v2.1/certs
- Scopes: openid, profile

## GitHub Pagesのリダイレクト先
https://yu16nk03-ux.github.io/nara-music-club/member/

Supabaseの Authentication > URL Configuration で、上記URLを Redirect URLs に追加してください。

## 注意
今回の版は「LINEログインが動くところ」までです。
次の段階で、以下をSupabaseに追加します。

- 初回ログイン時のメンバー承認
- 複数の運営メンバーによる管理
- 次回セッション参加曲・パート希望
- 希望者一覧の表示
- 回答締切
- 活動記録
- ライブ・出演情報

Publishable keyはブラウザで使える公開用キーですが、Secret keyは絶対にGitHub Pagesへ置かないでください。
