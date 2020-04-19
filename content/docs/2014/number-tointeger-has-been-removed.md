---
title: "`Number.toInteger()` has been removed"
date: "2014-07-22T05:06:26-04:00"
categories: ["javascript"]
tags: []
releases: ["33", "38-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1022396"
      title: "Bug 1022396 – remove Number.toInteger"
---
The [`Number.toInteger`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number/toInteger) method, implemented with Firefox 16, has been removed since it's no longer a part of the ES6 draft spec. [`Number.parseInt`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number/parseInt) can be used instead in most cases.
