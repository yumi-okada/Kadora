# ボタンコンポーネント詳細設計

## 1. 基本スタイル定義

- クラス名：`btn`
- 幅：160px
- 高さ：48px
- パディング：上下12px、左右24px
- 背景色：`#2563eb`
- 文字色：`#ffffff`（白）
- アニメーション効果：`transition: background-color 200ms ease, transform 100ms ease;`

## 2. インタラクション状態定義

- **Hover状態（:hover）**
  - マウスポインターが重なったとき、背景色を `#1d4ed8` に変更する。
  - カーソルを`cursor: pointer`で指の形に変更する。

- **Active状態（:active）**
  - `transform: scale(0.96)` でボタンを96％に縮小する

- **Focus状態（:focus）**
  - `outline: 3px solid #2563eb` で枠線を表示する
  - `outline-offset: 3px` でボタンと枠線の間隔を設定する
