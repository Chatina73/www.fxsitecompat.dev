---
title: "Calling `DataView` without `new` will throw"
date: "2015-04-27T13:17:23-04:00"
categories: ["javascript"]
tags: []
releases: ["40", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1142279"
      title: "Bug 1142279 – DataView should require `new`"
---
Firefox now throws a [`TypeError`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/TypeError) exception when the [`DataView`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/DataView) constructor is called without the [`new`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/new) operator, as per the specification.
