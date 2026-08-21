# nikki-pen

自分用の日記入力PWA。3フィールド（金・一行・メモ）を書いて「記す」を押すと、GitHubのprivateリポジトリ（日記の正本）へ直接コミットする。

- データはこのリポジトリには一切入らない。ここにあるのは皮（UI）だけ
- 認証はFine-grained PAT（対象リポ限定・Contents読み書きのみ）。端末のlocalStorageにのみ保存
- 圏外時はローカルにキューし、次回オンライン起動時に自動送信
- ホスティング: GitHub Pages（静的1ページ）

## セットアップ

1. GitHub Pagesを有効化（Settings → Pages → Deploy from a branch → main / root）
2. iPhoneのSafariでPages URLを開く → 共有 → **ホーム画面に追加**
3. 初回起動時に設定が開くので、Fine-grained PATを貼る

## v1スコープ

3フィールド＋保存＋オフラインキューのみ。履歴表示・装飾はv2以降（7日続いてから）。
