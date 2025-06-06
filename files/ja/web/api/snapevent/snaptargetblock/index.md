---
title: "SnapEvent: snapTargetBlock プロパティ"
short-title: snapTargetBlock
slug: Web/API/SnapEvent/snapTargetBlock
l10n:
  sourceCommit: 702cd9e4d2834e13aea345943efc8d0c03d92ec9
---

{{APIRef("Snap Events")}}{{SeeCompatTable}}

**`snapTargetBlock`** は {{domxref("SnapEvent")}} インターフェイスの読み取り専用プロパティで、このイベントが発行されたときに、ブロック方向にスナップされた要素への参照を返します。

具体的には、次のようになります。

- {{domxref("Element/scrollsnapchanging_event", "scrollsnapchanging")}} イベントの場合、これは待機中のブロック方向のスナップターゲット（つまり、現在のスクロール捜査が終了したときに選択されるもの）を参照します。
- {{domxref("Element/scrollsnapchange_event", "scrollsnapchange")}} イベントの場合、これは新しく選択されたブロック方向のスナップターゲットを参照します。

`SnapEvent` で利用可能なプロパティ値は、スクロールコンテナーに設定された {{cssxref("scroll-snap-type")}} プロパティの値に直接対応します。 `snapTargetBlock` は、スナップ軸が `block` （または、現在の書字方向で `block` に相当する物理軸値の場合）または `both` と指定されている場合、要素参照のみを返します。

## 値

スナップする要素を表す {{domxref("Node")}}、またはスクロールスナップがインライン方向でしか発生せず、ブロック方向にスナップされる要素がない場合は `null` です。

スナップされた要素が擬似要素であった場合、返される `Node` はその擬似要素を所有する要素です。

## 例

短い例については {{domxref("SnapEvent")}} のメインページを、完全な例と説明については[スクロールスナップイベントの使用](/ja/docs/Web/CSS/CSS_scroll_snap/Using_scroll_snap_events)ガイドを参照してください。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{domxref("Element/scrollsnapchanging_event", "scrollsnapchanging")}} イベント
- {{domxref("Element/scrollsnapchange_event", "scrollsnapchange")}} イベント
- [CSS スクロールスナップモジュール](/ja/docs/Web/CSS/CSS_scroll_snap)
- [Scroll Snap Events](https://developer.chrome.com/blog/scroll-snap-events) (developer.chrome.com, 2024)
