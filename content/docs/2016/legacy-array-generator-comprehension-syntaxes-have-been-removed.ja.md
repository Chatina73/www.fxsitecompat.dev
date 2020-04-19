---
title: "古い配列・ジェネレーター内包構文が削除されました"
date: "2016-01-07T01:11:00-05:00"
categories: ["javascript"]
tags: []
versions: ["46", "52-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1220564"
      title: "Bug 1220564 - Remove legacy array/generator comprehension."
aliases:
    - "/ja/docs/2015/array-generator-comprehensions-will-be-removed/"
    - "/ja/docs/2015/legacy-array-generator-comprehension-syntaxes-will-be-removed/"
---
JavaScript [1.7](https://developer.mozilla.org/docs/Web/JavaScript/New_in_JavaScript/1.7) と [1.8](https://developer.mozilla.org/docs/Web/JavaScript/New_in_JavaScript/1.8) で導入された古い非標準の [配列内包](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/Array_comprehensions#Differences_to_the_older_JS1.7JS1.8_comprehensions) と [ジェネレーター内包](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/Generator_comprehensions#Differences_to_the_older_JS1.7JS1.8_comprehensions) への対応は、Firefox 46 で削除されました。ECMAScript に提案されているそれぞれの新しい構文は Firefox 30 以降で使用可能となっています。ただし、それらが標準化されるかどうかは未だ不透明です。

**更新**: このドキュメントの初期草稿では配列・ジェネレーター内包が削除されると記載していましたが、バグが更新され、差し当たり古い構文のみ削除されることになりました。

**更新 2**: 新しい構文も標準化されなかったため、実装は [Firefox 58](https://www.fxsitecompat.dev/ja/docs/2017/array-generator-comprehension-support-has-been-removed/) で削除されました。
