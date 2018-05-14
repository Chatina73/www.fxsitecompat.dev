---
title: "`mozallowfullscreen` 属性の接頭辞が外れました"
date: "2012-12-03T03:53:26-05:00"
categories: ["dom"]
tags: []
versions: ["18"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=805301"
      title: "Bug 805301 – Rename mozallowfullscreen to allowfullscreen"
---
インラインフレーム ([`iframe`](https://developer.mozilla.org/docs/HTML/Element/iframe)) 内コンテンツの [全画面表示](https://developer.mozilla.org/docs/DOM/Using_fullscreen_mode) を許容する `mozallowfullscreen` 属性の接頭辞が外れました。HTML5 の `allowfullscreen` 属性は実際に *YouTube* の埋め込みプレーヤーで使用されています。
