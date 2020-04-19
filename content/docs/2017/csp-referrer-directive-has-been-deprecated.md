---
title: "CSP `referrer` directive has been deprecated"
date: "2017-03-10T16:09:00-05:00"
categories: ["dom", "privacy-security"]
tags: []
versions: ["52", "52-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1303682"
      title: "Bug 1303682 - Add deprecation warning before removing 'referrer' directive from CSP"
---
The Content Security Policy (CSP) [`referrer`](https://developer.mozilla.org/docs/Web/HTTP/Headers/Content-Security-Policy/referrer) directive, used to specify how the [`Referer`](https://developer.mozilla.org/docs/Web/HTTP/Headers/Referer) HTTP header works, is now deprecated and will be removed in the near future. It has already been removed from [Chrome 56](https://developers.google.com/web/updates/2016/12/chrome-56-deprecations) shipped this January. Use the [`Referrer-Policy`](https://developer.mozilla.org/docs/Web/HTTP/Headers/Referrer-Policy) HTTP header instead.

**Update**: The directive has been removed with [Firefox 62](https://www.fxsitecompat.dev/en-CA/docs/2018/csp-referrer-directive-has-been-removed/).
