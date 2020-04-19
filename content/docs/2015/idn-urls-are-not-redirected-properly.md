---
title: "IDN URLs are not redirected properly"
date: "2015-10-21T02:40:00-07:00"
categories: ["networking"]
tags: []
releases: ["36", "42"]
statuses: "regressed"
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1142083"
      title: "Bug 1142083 - IDN Unicode domain redirect is broken in Firefox 36/37/38"
---
Firefox 36 has a regression where URLs containing a Unicode-format [internationalized domain name](https://en.wikipedia.org/wiki/Internationalized_domain_name) (IDN) are not redirected properly, leading to a Server Not Found error. This bug has been fixed with Firefox 41 but still remains in 42 and later.

**Update**: This bug has been fixed again with Firefox 45.
