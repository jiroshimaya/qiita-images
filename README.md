# qiita-images

Qiita記事で使う画像のホスティング用リポジトリ。記事本体は別リポジトリ(qiita-content)で管理し、
画像はここに置いて [jsDelivr](https://www.jsdelivr.com/) 経由の安定URLで参照する。

参照例:
`https://cdn.jsdelivr.net/gh/jiroshimaya/qiita-images@main/fictional-scientists/<記事>/<ファイル>`

同じパスの画像を更新して push すると、記事側の画像も更新される(jsDelivrのキャッシュは
`https://purge.jsdelivr.net/gh/...` で明示パージ可能)。
