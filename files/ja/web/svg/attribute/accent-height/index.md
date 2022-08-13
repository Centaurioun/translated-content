---
title: accent-height
slug: Web/SVG/Attribute/accent-height
tags:
  - Deprecated
  - NeedsExample
  - SVG
  - SVG Attribute
translation_of: Web/SVG/Attribute/accent-height
---
{{SVGRef}}{{deprecated_header}}

**`accent-height`**属性は原点からアクセント文字の上端までの距離を定義します。これはフォント座標系で測られる距離です。

1 つの要素のみがこの属性を使用します: {{SVGElement("font-face")}}

## font-face

{{SVGElement("font-face")}}に対して、`accent-height`は原点からアクセント文字の上端までの距離を定義します。これはフォント座標系で測られる距離です。

| 値                 | [<number>](/ja/docs/Web/SVG/Content_type#Number) |
| ------------------ | ------------------------------------------------ |
| 既定値             | Value of {{SVGAttr("ascent")}}            |
| アニメーション可否 | いいえ                                           |

## 仕様

| 仕様書                                                                                                                   | 策定状況                 | コメント |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------ | -------- |
| {{SpecName("SVG1.1", "fonts.html#FontFaceElementAccentHeightAttribute", "accent-height")}} | {{Spec2("SVG1.1")}} | 初期定義 |

## ブラウザー実装状況

{{Compat("svg.elements.font-face.accent-height")}}

## 関連情報

- {{SVGAttr("cap-height")}}
- {{SVGAttr("x-height")}}