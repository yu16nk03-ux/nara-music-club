# NMC v2.5 LINEログイン設定

## 今回入った機能
- LINEログイン
- Supabase Authとの接続
- `members` テーブルの会員確認
- `approved = true` の会員だけ会員画面を表示
- `approved = false` は承認待ち表示
- `is_admin` はDBから取得（今後の管理者画面で利用）

## まだ1回だけ設定が必要
`member/index.html` の以下2項目をSupabaseの値に置き換えてください。

```js
const SUPABASE_URL="YOUR_SUPABASE_PROJECT_URL";
const SUPABASE_PUBLISHABLE_KEY="YOUR_SUPABASE_PUBLISHABLE_KEY";
```

- SUPABASE_URL：Data APIのAPI URL
- SUPABASE_PUBLISHABLE_KEY：Project Settings → API Keys → Publishable key

⚠️ Secret key / service_role key は絶対に入れないでください。

## GitHub Pagesのログイン戻り先
https://yu16nk03-ux.github.io/nara-music-club/member/

Supabaseの Authentication → URL Configuration で、必要なら上記URLを Redirect URLs に追加してください。

## 次の段階
LINEログインが成功したら、
1. 曲登録
2. 曲ごとのパート希望
3. 他メンバーの希望状況表示
4. 回答締切（前日まで）
5. 活動記録
6. ライブ・出演情報
7. 管理者画面
を追加します。
