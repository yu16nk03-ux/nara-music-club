# NMC v3.6 セットアップ

## 今回の修正
初めてLINEログインした人を `members` テーブルへ自動登録します。

流れ：
1. LINEでログイン
2. `members` に未登録なら自動登録
3. `approved = false` で承認待ち
4. 運営管理画面の「👥 メンバー承認」に表示
5. 運営が「承認する」
6. MEMBERページを利用可能

## 1回だけSupabaseでSQLを実行
Supabase → SQL Editor → New query を開き、
`NMC-v3.6-Supabase-member-auto-registration.sql` の内容を貼り付けて Run。

## その後
ZIPの中身をGitHub Pagesへアップロードしてください。

### 注意
- 既存の承認済みメンバーには影響しません。
- 新規ユーザーは自動的に承認待ちになります。
- `approved` と `is_admin` は新規登録時に false です。
