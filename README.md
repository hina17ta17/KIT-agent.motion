# kit-agent モーションスタジオ

kit-agent の動きを見るための、一枚の頁です。

**見るところ** → https://hina17ta17.github.io/KIT-agent.motion/

## 中に何が入っているか

| ファイル | 何か |
|---|---|
| `kit-agent-motion.html` | 本体。頁そのもの |
| `index.html` | 根っこの住所を開いた人を、本体へ送るだけのもの |
| `kit-agent-model.jpeg` | 頁の中で出る、kit-agent のモデルの写真 |
| `.nojekyll` | GitHub Pages に、余計な組み立てをさせないための印 |

## なぜ index.html が要るか

GitHub Pages は、住所の最後が `/` のとき `index.html` を探します。
`kit-agent-motion.html` だけを置くと、根っこの住所には何も無いので
**404** になります（ファイルの名前まで打てば開ける、という状態）。

本体の名前を変えると、すでに配った住所が切れてしまうので、
名前は変えずに `index.html` を足してあります。どちらの住所からも開けます。

## 写真について

頁の中で `kit-agent-model.jpeg` を読んでいます。
この写真が入っていないと、そこだけ何も出ません
（`onerror` で隠れるので、崩れはしませんが、消えます）。
写真を差し替えるときは、同じ名前で置き換えてください。

## 直したものを、どうやって出すか

`main` に入れると、GitHub Pages がそのまま出します（Settings → Pages が
`main` / `(root)` を見ています）。出るまでに、少し待つことがあります。
