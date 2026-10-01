# kit-agent モーションスタジオ

kit-agent の動きを見るための、一枚の頁です。

**見るところ** → https://hina17ta17.github.io/KIT-agent.motion/

## 中に何が入っているか

| ファイル | 何か |
|---|---|
| `index.html` | **本体。頁そのもの** |
| `kit-agent-motion.html` | 前の名前。短いほうの住所へ送るだけ |
| `kit-agent-model.jpeg` | 頁の中で出る、kit-agent のモデルの写真 |
| `.nojekyll` | GitHub Pages に、余計な組み立てをさせないための印 |

## 住所は一本

GitHub Pages は、住所の最後が `/` のとき `index.html` を探します。
だから本体を `index.html` にしておけば、

    https://hina17ta17.github.io/KIT-agent.motion/

これだけで頁が出ます。ファイルの名前を打つ必要はありません。

前は本体が `kit-agent-motion.html` で、`index.html` はそこへ送るだけの
ものでした。その形だと、短い住所で開いても画面の住所が長いほうへ
変わってしまいます。中身と住所を入れ替えて、短いほうを本体にしました。

`kit-agent-motion.html` は消していません。すでに配った住所が切れないよう、
短いほうへ送るだけのものとして残してあります。

**直すときは `index.html` を直してください。**

## 写真について

頁の中で `kit-agent-model.jpeg` を読んでいます。
この写真が入っていないと、そこだけ何も出ません
（`onerror` で隠れるので、崩れはしませんが、消えます）。
写真を差し替えるときは、同じ名前で置き換えてください。

## 直したものを、どうやって出すか

`main` に入れると、GitHub Pages がそのまま出します（Settings → Pages が
`main` / `(root)` を見ています）。出るまでに、少し待つことがあります。

## 検索に載せていません

`index.html` と `kit-agent-motion.html` の頭に
`<meta name="robots" content="noindex, nofollow">` を入れてあります。
住所を知っている人は開けますが、検索からは辿り着きません。

載せたくなったら、その一行を消してください。
（`robots.txt` はこの置き場では効きません。読まれるのは
`hina17ta17.github.io/robots.txt` だけで、レポジトリの中に置いても見てもらえません）

## 中の絵と頁について

この頁と、`kit-agent-model.jpeg` は作者のものです。
公開の場所に置いてある以上、開いた人は保存できます。
転載や二次利用はご遠慮ください。

## 置いてある人へ

コミットに入る作者のアドレスは、公開レポジトリでは誰にでも見えます。
大学のアドレスは学籍番号を含むので、GitHub の noreply
（`…@users.noreply.github.com`）を使ってください。

    git config --global user.email "…@users.noreply.github.com"

あわせて GitHub の Settings → Emails で
「Keep my email addresses private」と
「Block command line pushes that expose my email」を入れておくと、
うっかり出すことがなくなります。
