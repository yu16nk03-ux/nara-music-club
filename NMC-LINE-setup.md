# NMC v2.4 — LINEログイン準備版

`/member/` にNMC MEMBERのLINEログイン画面を追加しました。
Supabase Custom Provider `custom:line` を呼び出す準備まで入っています。

次に `member/index.html` の以下2項目へ、SupabaseのProject URLとPublishable keyを設定します。
- YOUR_SUPABASE_PROJECT_URL
- YOUR_SUPABASE_PUBLISHABLE_KEY

Secret key / service_role keyはブラウザ側へ入れないでください。

この版はLINEログイン呼び出しまでの準備版です。
承認待ち・承認済み会員ページ・曲/パート希望・活動記録・管理画面は次段階でDB/RLSと合わせて実装します。
