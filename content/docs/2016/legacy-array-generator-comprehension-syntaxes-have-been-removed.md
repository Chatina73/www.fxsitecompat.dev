---
title: "Legacy array/generator comprehension syntaxes have been removed"
date: "2016-01-07T01:11:00-05:00"
categories: ["javascript"]
tags: []
versions: ["46"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1220564"
      title: "Bug 1220564 - Remove legacy array/generator comprehension."
aliases:
    - "/en-CA/docs/2015/array-generator-comprehensions-will-be-removed/"
    - "/en-CA/docs/2015/legacy-array-generator-comprehension-syntaxes-will-be-removed/"
---
The support for the legacy, non-standard [array comprehensions](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/Array_comprehensions#Differences_to_the_older_JS1.7JS1.8_comprehensions) and [generator comprehensions](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Operators/Generator_comprehensions#Differences_to_the_older_JS1.7JS1.8_comprehensions), introduced with JavaScript [1.7](https://developer.mozilla.org/docs/Web/JavaScript/New_in_JavaScript/1.7) and [1.8](https://developer.mozilla.org/docs/Web/JavaScript/New_in_JavaScript/1.8) respectively, has been removed with Firefox 46. Each new syntax proposed for ECMAScript is available since Firefox 30, though it's still uncertain whether those will be standardized.

**Update**: The initial draft of this document said array/generator comprehensions would be removed, but the bug has been updated to only remove the legacy syntaxes for now.

**Update 2**: The newer syntaxes couldn't be standardized either, and therefore, the implementation has been removed with [Firefox 58](https://www.fxsitecompat.dev/en-CA/docs/2017/array-generator-comprehension-support-has-been-removed/).
