---
title: "Evaluation order of default parameters and functions inside function body is changed"
date: "2014-07-22T05:06:26-04:00"
categories: ["javascript"]
tags: []
versions: ["33"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1022962"
      title: "Bug 1022962 – Default parameters should be evaluated before function declarations"
---
[Default parameters](https://developer.mozilla.org/docs/Web/JavaScript/Reference/default_parameters), implemented with Firefox 15, were evaluated after functions inside the function body, but now are evaluated before those functions. So those functions cannot be referred from default parameters.
