---
marp: true
theme: sample
header: "**ヘッダータイトル1** __ヘッダータイトル2__"
footer: "by **xianglishan**"
paginate: true
backgroundColor: white

---
# :+1:Marpのtest<!-- omit in toc -->
themeはデフォで3種類(これは今はgaia)
- theme: default
- theme: gaia
- theme: uncover

cssをカスタムテーマとして使うこともできる(後述)
Ctrl+Shift+P -> markdown toc で目次作成
`# aaa`とかって書くと勝手に目次作ってくれる。
`# aaa<!-- omit in toc -->`って書くと目次から除外

--- 
###  目次<!-- omit in toc -->
- [前提として](#前提として)
- [参照](#参照)
- [cssのあてかたとか](#cssのあてかたとか)
- [文字](#文字)
- [cssあてる](#cssあてる)
  - [aa](#aa)
- [画像の置き方とか](#画像の置き方とか)
- [サブタイトル](#サブタイトル)
- [draw.ioとかのSVGをおく](#drawioとかのsvgをおく)

---
##  前提として
- vscodeのmarp拡張使う
- pptx, pdf にexportは右上のMarpボタン

---
## 参照
- 絵文字は以下参照
https://gist.github.com/spiegel-im-spiegel/66aac732f27ad69cc8b6bd33478ecfa4
- 以下最強のレファレンス
    - [Qiit 【VS Code + Marp】Markdownから爆速・自由自在なデザインで、プレゼンスライドを作る](https://qiita.com/tomo_makes/items/aafae4021986553ae1d8#drawio )
    - [Qiita Marp(Marpit)](https://qiita.com/takeshisakuma/items/5a61e6eac123d28602fb#%E3%83%86%E3%83%BC%E3%83%9E%E3%81%AE%E3%82%B5%E3%83%B3%E3%83%97%E3%83%AB)
    - [Qiita （備忘録）Marpテンプレート](https://qiita.com/zono_0/items/e6ab64f381440578ea1c)

---
## cssのあてかたとか
- 左下の管理ボタン:gear:→設定(Ctrl+,)
- marp themeで検索してcssのパス指定でカスタムテーマを追加する
↓こんな感じ
![](./images/スクリーンショット%202021-10-18%20034404.png)

---
## 文字
- 普通に書いて`---`で区切ると改ページ
- あとは普通のmarkdown的にかけるよ

## cssあてる
- cssファイル用意
- vscodeの設定全ページ
- 本ファイルの先頭にtheme: hoge

---
<!--
class: heading
-->

# 見出し1<!-- omit in toc -->
## 見出し2<!-- omit in toc -->
### 見出し3<!-- omit in toc -->
#### 見出し4<!-- omit in toc -->
##### 見出し5<!-- omit in toc -->
###### 見出し6<!-- omit in toc -->

---
<!--
_class: lists
-->
### aa
- 要素1
- 要素2
- 要素3

---
<!--
_class: paragraph
-->
パラグラフ
- `<!-- hoge -->`のときは以降すべてのスライドにcssあてる
- `<!-- _hoge -->`のときは該当スライドのみ

---
ソースコード等は
```bash
$hoge = rand(1, 4)
```

---
##  画像の置き方とか
markdown的に書いたらいい感じになる。
以降のページを参照

---
<!-- bgで画像を背景に設定し、fitで画像のサイズを自動調整 -->
![bg fit](https://placehold.jp/400x400.png)

---
<!-- rightで右寄せ -->
## サブタイトル
- 多分
- こんな感じで
- 右図の説明とかを書く
list以外も普通にかけるよ
![bg right](https://placehold.jp/400x400.png)

---
<!-- leftで左寄せ -->
![bg left](https://placehold.jp/400x400.png)

---
<!-- 画像を縦に並べる -->
![bg fit vertical right](https://placehold.jp/400x400.png)
![bg fit vertical right](https://placehold.jp/400x400.png)

---
<!-- 画像のサイズを%で指定。透明度も設定 -->
![bg 40% opacity:.3](https://placehold.jp/400x400.png)

---
<!-- 画像を横に2枚並べたい時 -->
![](https://placehold.jp/400x400.png) ![](https://placehold.jp/400x400.png)

---
## draw.ioとかのSVGをおく
多分こんな感じで説明入れたり

![bg right 50%](./drawio/test.drawio.svg)