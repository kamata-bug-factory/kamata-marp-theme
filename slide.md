---
marp: true
theme: kamata-theme
paginate: true
---

<!-- _class: title -->
<!-- _paginate: false -->

<br>

# テーマ機能網羅デモ用スライド

鎌田 一輝

---

<!-- _class: section -->
<!-- _paginate: false -->

### Part 1

## 基本要素の確認

#### テキスト・リスト・コードなど基本マークダウン要素

---

# 見出し (Headings)

<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

---

# テキストスタイル

標準のテキストです。色は `--gray-medium` です。

- **Bold text (strong)**: 太字で強調
- _Italic text (em)_: 斜体で強調
- <small>Small text (small)</small>: 注釈などに使用
- [Link text](https://example.com): リンクの色は `--accent-primary`

> Blockquote: 引用文のスタイルです。
> 左側にボーダーが付きます。

---

# リスト (Lists)

- Unordered List Item 1
- Unordered List Item 2
  - Nested Item 2.1
  - Nested Item 2.2

1. Ordered List Item 1
2. Ordered List Item 2
   1. Nested Item 2.1
   2. Nested Item 2.2

---

# コードブロックとテーブル

インラインコード: `const a = 1;`

```javascript
// Code block
function hello() {
  console.log("Hello, Marp!");
}
```

| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Left     |  Center  |    Right |
| Item 1   |  Item 2  |   Item 3 |
| Item 4   |  Item 5  |   Item 6 |

---

# Small Text Class

<!-- _class: small-text -->

このスライドは `small-text` クラスが適用されています。
全体のフォントサイズが約20%縮小されます。

- 通常のスライドよりも多くの情報を詰め込むことができます。
- リストの行間なども調整されています。

```python
def example():
    return "Code block font size is also smaller"
```

---

<!-- _class: section -->
<!-- _paginate: false -->

### Part 2

## レイアウトバリエーション

#### カラム・グリッド・画像配置など

---

<!-- _class: no-header -->

# No Header Class

このスライドは `no-header` クラスが適用されています。
上部のヘッダー領域（ページ番号やフッター以外の装飾）が非表示または調整され、パディングが変わります。

---

<!-- _class: align-center -->

# Align Center

このスライドは `align-center` クラスが適用されています。
コンテンツが垂直方向に中央揃えになります。

---

<!-- _class: all-text-center -->

# All Text Center

このスライドは `all-text-center` クラスが適用されています。
すべてのテキストが中央揃えになります。

- リストアイテムも
- 中央に
- 配置されます

---

<!-- _class: column-layout-2 -->

# Column Layout 2

<div class="column">

## Left Column

`column-layout-2` クラスと `div.column` を使用して2カラムレイアウトを実現します。

- 左側のコンテンツ
- リストなども配置可能

</div>

<div class="column">

## Right Column

右側のカラムです。カラム内では h1 もヘッダーバーにならず通常の見出しとして表示されます。

</div>

---

<!-- _class: toc -->

# 目次 (TOC)

1. **基本要素の確認**
   テキスト・リスト・コードなど
1. **レイアウトバリエーション**
   カラム・グリッド・画像配置
1. **カラーバリエーション**
   テキストカラーユーティリティ
1. **画像レイアウト**
   image / content-image 系クラス

---

<!-- _class: grid -->

# Grid レイアウト

<div class="cell">

## フロントエンド

- React / Next.js
- TypeScript
- Tailwind CSS

</div>

<div class="cell">

## バックエンド

- Node.js
- Python / FastAPI
- PostgreSQL

</div>

<div class="cell">

## インフラ

- AWS Lambda
- DynamoDB
- CloudFront

</div>

<div class="cell">

## ツール

- GitHub Actions
- Docker
- Terraform

</div>

---

<!-- _class: section -->

### Part 3

## カラーバリエーション

#### テキストカラーユーティリティ

---

<!-- _class: all-text-teal -->

# All Text Teal

このスライドは `all-text-teal` クラスが適用されています。
すべてのテキストがティール（`--accent-primary`）になります。

- リストアイテムもティール色
- **強調**もティールベース

---

<!-- _class: all-text-amber -->

# All Text Amber

このスライドは `all-text-amber` クラスが適用されています。
すべてのテキストがアンバー（`--accent-secondary`）になります。

重要事項の伝達などに使用できます。

---

<!-- _class: h1-text-center h2-text-teal -->

# 個別見出しユーティリティ

## h2 だけティールカラー

`h1-text-center` で h1 のみ中央揃え、`h2-text-teal` で h2 のみティールカラーに変更できます。

個別見出しユーティリティは `h1`〜`h6` の各レベルに対応しています。

---

<!-- _class: text-center text-amber -->

# Text Center + Text Amber

`text-center` は段落テキストのみ中央揃え、`text-amber` は段落テキストのみアンバーカラーにします。

見出しには適用されません。

---

<!-- _class: section -->

### Part 4

## 画像レイアウト

#### image / content-image 系クラス

---

<!-- _class: image -->

# Image Class

`image` クラス: 画像を配置するための基本クラス

![w:600](https://placehold.co/600x400/png)

---

<!-- _class: content-image -->

# Content Image

> `content-image` クラス: テキストと画像を混在させるレイアウト。テキストは blockquote 形式で記述する。

![w:500](https://placehold.co/500x300/png)

---

<!-- _class: content-image-right -->

# Image Right (50%)

`content-image-right`

右半分に画像が配置されます。
テキストは左側に配置されます。

![w:800](https://placehold.co/800x600/1a7a6d/ffffff?text=Right+Image)

---

<!-- _class: content-image-right content-30 -->

# Image Right (30%)

`content-image-right` + `content-30`

画像エリアが30%になります。
テキストエリアが広くなります。

![w:400](https://placehold.co/400x600/c47a2a/ffffff?text=30%25)

---

<!-- _class: content-image-left -->

# Image Left (50%)

`content-image-left`

左半分に画像が配置されます。
テキストは右側に配置されます。

![w:800](https://placehold.co/800x600/3e3a36/ffffff?text=Left+Image)

---

<!-- _class: content-image-left content-70 -->

# Image Left (70%)

`content-image-left` + `content-70`

画像エリアが70%になります。
テキストエリアは狭くなります。

![w:1000](https://placehold.co/1000x600/2d2926/ffffff?text=70%25)

---

<!-- _class: image-shadow -->

# Image Shadow

`image-shadow` クラス

画像に影（ドロップシャドウ）がつきます。

![w:600](https://placehold.co/600x400/ffffff/000000?text=Shadow+Effect)

---

<!-- _class: title -->
<!-- _paginate: false -->

<br>

# ご清聴ありがとうございました

<br>
