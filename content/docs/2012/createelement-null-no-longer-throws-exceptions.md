---
title: "`createElement(null)` no longer throws exceptions"
date: "2012-12-03T03:54:45-05:00"
categories: ["dom"]
tags: []
versions: ["19", "24-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=802562"
      title: "Bug 802562 – createElement(null) should work like createElement(\"null\")"
---
Previously the [`document.createElement`](https://developer.mozilla.org/docs/Web/API/document.createElement) method has thrown exception `INVALID_CHARACTER_ERR` if the argument was `null`. The method now returns the [`HTMLUnknownElement`](https://developer.mozilla.org/docs/Web/API/HTMLUnknownElement) object because the argument should be treated as a string and considered to be the same code as `document.createElement("null")`.
