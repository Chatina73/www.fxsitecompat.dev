---
title: "`__noSuchMethod__` has been deprecated"
date: "2015-03-17T14:02:59-04:00"
categories: ["javascript"]
tags: []
versions: ["39", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=683218"
      title: "Bug 683218 - can we remove __noSuchMethod__, use proxies instead?"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1140428"
      title: "Bug 1140428 - Warn when __noSuchMethod__ is used"
---
The non-standard [`Object.prototype.__noSuchMethod__`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object/noSuchMethod) property is now considered deprecated and will be removed in the near future. It raises a warning in the [Web Console](https://developer.mozilla.org/docs/Tools/Web_Console) from now on. The standard [`Proxy`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Proxy) object defined in the ECMAScript 6 specification can be used instead.

**Update**: The `__noSuchMethod__` support has been [removed with Firefox 44](https://www.fxsitecompat.dev/en-CA/docs/2015/nosuchmethod-is-no-longer-supported/).
