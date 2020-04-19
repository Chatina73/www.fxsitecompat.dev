---
title: "`Map.size()` and `Set.size()` have been changed to properties"
date: "2012-12-03T03:54:45-05:00"
categories: ["javascript"]
tags: []
releases: ["19", "24-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=807001"
      title: "Bug 807001 – Map.prototype.size and Set.prototype.size should be accessor properties"
---
The `size` method, that returns the number of key/value pairs saved in a [`Map`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Map) object and the number of values saved in a [`Set`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Set) object, are changed to be read-only properties.
