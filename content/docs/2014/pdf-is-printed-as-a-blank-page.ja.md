---
title: "PDF が空白のページとして印刷されます"
date: "2014-02-07T11:57:09-05:00"
categories: ["misc"]
tags: []
versions: ["29"]
statuses: "regressed"
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1003707"
      title: "Bug 1003707 – pdf.js print prints a white page"
---
PDF.js と呼ばれる Firefox の組み込み PDF ビューアで PDF ファイルを印刷すると、プリンター出力が空白のページとなってしまいます。このリグレッションは Firefox 29.0.1 で修正されました。
