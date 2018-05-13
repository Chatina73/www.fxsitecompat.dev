---
title: "Scroll-linked positioning effects may not work well with async scrolling, console warns"
date: "2016-01-07T09:01:00-05:00"
categories: ["javascript"]
tags: []
versions: ["46"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1229052"
      title: "Bug 1229052 - Log a warning if webpage is updating positioning properties during a scroll event listener"
    - url: "https://hacks.mozilla.org/2016/02/smoother-scrolling-in-firefox-46-with-apz/"
      title: "Mozilla Hacks - Smoother scrolling in Firefox 46 with APZ"
---
Starting with Firefox 46, the Web Console warns page scripts altering scroll positioning properties in a [`scroll`](https://developer.mozilla.org/docs/Web/Events/scroll) event listener. Such event handlers are often used for sticky element positioning, scroll snapping or parallax effects, but may not work well with asynchronous scrolling being implemented in Firefox. See the [Scroll-Linked Effects](https://developer.mozilla.org/docs/Mozilla/Performance/ScrollLinkedEffects) page on MDN for details and possible workarounds.
