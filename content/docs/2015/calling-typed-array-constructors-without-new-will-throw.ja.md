---
title: "`new` なしで型付き配列コンストラクターを呼び出すと例外が投げられます"
date: "2015-10-14T16:00:00-07:00"
categories: ["javascript"]
tags: []
versions: ["44", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=980945"
      title: "Bug 980945 - Typed array constructors should not work without \"new\" per spec"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1214936"
      title: "Bug 1214936 - Make the ArrayBuffer constructor throw if invoked without 'new'"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1062075"
      title: "Bug 1062075 - Throw for ES6 built-in constructors called without `new`"
---
ECMAScript 2015 (ES6) 準拠の一環として、[`Uint8Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Uint8Array)、[`Int16Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Int16Array)、[`Float64Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Float64Array) などの [型付き配列](https://developer.mozilla.org/docs/Web/JavaScript/Typed_arrays) コンストラクターのいずれか、あるいは [`ArrayBuffer`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/ArrayBuffer) が [`new`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/new) 演算子なしで呼び出された場合に、Firefox は [`TypeError`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/TypeError) を投げるようになりました。

これにより、すべての組み込み ES6 コンストラクターが `new` なしで呼び出された場合に例外を投げるようになりました。
