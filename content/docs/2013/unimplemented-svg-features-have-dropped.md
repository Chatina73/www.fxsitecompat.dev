---
title: "Unimplemented SVG features have dropped"
date: "2013-02-06T08:44:10-05:00"
categories: ["svg"]
tags: []
versions: ["21"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=824218"
      title: "Bug 824218 – Remove unimplemented SVG features"
---
Unimplemented SVG features have been removed instead of just returning the `NOT_IMPLEMENTED` errors. These features include the `viewport` and `currentView` properties of [`SVGSVGElement`](https://developer.mozilla.org/docs/Web/API/SVGSVGElement).
