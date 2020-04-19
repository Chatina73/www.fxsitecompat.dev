---
title: "Service Worker Cache API added several global objects"
date: "2015-06-13T15:20:46-04:00"
categories: ["dom"]
tags: []
versions: ["41", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=940273"
      title: "Bug 940273 - Implement Cache and CacheStorage for ServiceWorkers"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1110144"
      title: "Bug 1110144 - ship Service Worker Cache in release builds"
---
Firefox 39 has enabled the [Service Worker](https://developer.mozilla.org/docs/Web/API/ServiceWorker_API) Cache API by default. This API provides the new [`Cache`](https://developer.mozilla.org/docs/Web/API/Cache) and [`CacheStorage`](https://developer.mozilla.org/docs/Web/API/CacheStorage) interfaces as well as the global [`caches`](https://developer.mozilla.org/docs/Web/API/WorkerGlobalScope/caches) property, so that you can no longer use those names for your own global variables.
