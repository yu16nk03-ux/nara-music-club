NMC v3.4 — 管理画面修正版＋ホームページ自動連携

# Nara Music Circle Website v2.1

Nara Music Circleのホームページ v2.1です。GitHub Pagesで公開できます。

## アップロード
リポジトリ直下に `index.html`、`style.css`、`script.js`、`images`、`member` を配置してください。

## 今回の変更
- 温かみのあるベージュを基調にしたデザインへ調整
- スマートフォン向けレイアウトを改善
- NMCの紹介文・メッセージ・Q&Aを更新
- 「こんな方におすすめです」を追加
- Instagram DMへの導線とDM例を追加
- ギャラリーのサイズを統一し、クリックで拡大表示できるように変更
- メンバー専用ページの入口を追加
- 文章全体を柔らかいNMCらしい言葉づかいに統一

## Instagram
https://www.instagram.com/nmc_official_2026/

## 注意
`member/` は現時点では「入口ページ」です。GitHub Pagesだけでは安全な会員限定認証はできないため、実際の会員情報をここへ直接置かないでください。Notion等を使った会員管理・認証方式を決めた段階で接続します。


## v3.2
活動記録に写真・活動メモ・YouTube限定公開動画を追加しました。Supabaseで `NMC-v3.2-Supabase-activity.sql` を実行してください。


## v3.6
初回LINEログインしたユーザーをmembersへ自動登録し、運営の承認待ちにする修正です。Supabaseで `NMC-v3.6-Supabase-member-auto-registration.sql` を1回実行してください。


【v3.8】YouTubeの通常動画URLに加えて、YouTubeプレイリストURL（youtube.com/playlist?list=...）も活動記録・ライブ出演情報で登録・表示できるようにしました。

## v3.9 変更
- メンバー側の活動記録・ライブ/出演情報でYouTube動画/プレイリストへのリンクを表示。
- 写真を最大4枚だけカード内に表示し、タップ/「写真をすべて見る」で全写真を確認可能。
- v3.9はフロント側の変更のみで、追加SQLは不要。
