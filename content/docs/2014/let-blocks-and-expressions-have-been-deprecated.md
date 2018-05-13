---
title: "`let` blocks and expressions have been deprecated"
date: "2014-12-19T11:15:21-05:00"
categories: ["javascript"]
tags: []
versions: ["36"]
cclicense: "BY-SA 3.0"
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1023609"
      title: "Bug 1023609 – Delete support for let blocks and let expressions for ES6"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1102131"
      title: "Bug 1102131 – Log warnings and collect telemetry for deprecated let blocks and let expressions"
---
The non-standard [`let` blocks and `let` expressions](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/let#Non-standard_let_extensions) are now considered deprecated. The support for those `let` extensions, currently warned in the [Web Console](https://developer.mozilla.org/docs/Tools/Web_Console), will be removed from Firefox in the near future.

**Update**: The `let` expression support has been [removed with Firefox 41](https://www.fxsitecompat.com/en-CA/docs/2015/let-expression-support-has-been-dropped/).

**Update**: The `let` block support will be [removed with Firefox 44](https://www.fxsitecompat.com/en-CA/docs/2015/let-block-support-will-be-dropped/) at earliest.
