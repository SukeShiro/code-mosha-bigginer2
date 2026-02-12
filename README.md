# CodeJump 模写コーディング（初級）

## 概要
CodeJump 初級課題「Store2」をもとに制作した模写コーディング作品です。

デザインの再現だけでなく、
・レイアウト設計
・レスポンシブ対応
・hoverアニメーションの実装
を意識して制作しました。

## 公開URL
https://sukeshiro.github.io/code-mosha-bigginer2/

---

## コーディング仕様

- フォント  
  Arial, Hiragino Sans, Hiragino Kaku Gothic ProN, Meiryo, sans-serif

- コンテンツ幅  
  max-width: 1200px  
  左右padding: 5%

- ブレークポイント  
  896px

---

## 実装ポイント

### 1. レイアウト設計
- コンテンツ幅（1200px）と全幅背景を分離
- Archive / New は grid を使用
- Catalog / Antique は flex を使用し、SPでは縦積みに変更

### 2. hover表現
- Archive / New は疑似要素 `::before` を使用し、
  画像のみ暗転させる設計にしました。
- ボタンは `::before` を使い、背景変化を実装。

### 3. レスポンシブ対応
- PCでは2カラム構成
- SPでは block レイアウトへ変更
- max-width 制限を解除し自然な縦積みへ調整

---

## 使用技術
- HTML
- CSS
  - grid
  - flexbox
  - aspect-ratio
  - 擬似要素 (::before)
  - media query

---

## 制作意図

デザインを再現するだけでなく、
「どの要素を親にするか」
「どこをflexにするか」
「どのhoverが適切か」
を設計しながら実装しました。

模写を通して、
再現力だけでなく構造理解を高めることを目的としています。
