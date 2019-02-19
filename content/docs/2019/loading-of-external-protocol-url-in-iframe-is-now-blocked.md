---
title: "Loading of external protocol URL in `<iframe>` is now blocked"
date: "2019-02-18T21:28:00-05:00"
categories: ["misc"]
tags: []
versions: ["66"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=167475"
      title: "Bug 167475 - [URL] Disable external and returning no data protocol handlers in all cases, excluding <A HREF=>"
---
On Firefox 66 and later, in order to avoid DoS-like attacks, external protocol URLs that don't return any data can no longer be loaded in an `<iframe>`. The affected protocols include `mailto` that could be used to open an email client, as shown below:

```html
<!-- This kind of URLs will be blocked from now on -->
<iframe src="mailto:support@example.com"></iframe>
<iframe src="ircs://irc.mozilla.org/firefox"></iframe>
<iframe src="itms://itunes.apple.com/us/app/apple-store/id989804926"></iframe>
```

Regular links like `<a href="mailto:...">` and JavaScript code like `location.href='mailto:...'` will continue working.