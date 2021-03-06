---
description: 最適化されたページには、静的に最適化されているかどうかを知らせるインジケーターが含まれています。また、こちらでオプトアウトすることができます。
---

# 静的最適化インジケータ

> **注意:** このインジケーターはバージョン 10.0.1 で削除されました。Next.js の最新バージョンにアップグレードすることを推奨します。

ページが [Automatic Static Optimization](/docs/advanced-features/automatic-static-optimization.md) の対象となる場合は、インジケーターを表示してお知らせします。

Automatic Static Optimization 自体とても有益なものですし、ページが Automatic Static Optimization の対象であるか開発時にすぐ分かるので、これは役に立ちます。

しかし、 Electron アプリケーションで動かすときなど、インジケーターは役に立たない場合があります。インジケーターを削除するためには、`next.config.js` ファイルを開き、`devIndicators` プロパティの `autoPrerender` 設定を無効にします:

```js
module.exports = {
  devIndicators: {
    autoPrerender: false
  }
};
```
