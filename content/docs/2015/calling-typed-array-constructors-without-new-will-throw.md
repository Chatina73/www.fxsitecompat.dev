---
title: "Calling typed array constructors without `new` will throw"
date: "2015-10-14T16:00:00-07:00"
categories: ["javascript"]
tags: []
versions: ["44"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=980945"
      title: "Bug 980945 - Typed array constructors should not work without \"new\" per spec"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1214936"
      title: "Bug 1214936 - Make the ArrayBuffer constructor throw if invoked without 'new'"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1062075"
      title: "Bug 1062075 - Throw for ES6 built-in constructors called without `new`"
---
As part of the ECMAScript 2015 (ES6) compliance, Firefox now throws a [`TypeError`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/TypeError) if one of the [typed array](https://developer.mozilla.org/docs/Web/JavaScript/Typed_arrays) constructors, including [`Uint8Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Uint8Array), [`Int16Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Int16Array) and [`Float64Array`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Float64Array), or [`ArrayBuffer`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/ArrayBuffer) is called without using the [`new`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/new) operator.

All built-in ES6 constructors are hereby throwing when called without `new`.
