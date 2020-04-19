---
title: "`__noSuchMethod__` が廃止予定となりました"
date: "2015-03-17T14:02:59-04:00"
categories: ["javascript"]
tags: []
releases: ["39", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=683218"
      title: "Bug 683218 - can we remove __noSuchMethod__, use proxies instead?"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1140428"
      title: "Bug 1140428 - Warn when __noSuchMethod__ is used"
---
非標準の [`Object.prototype.__noSuchMethod__`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object/noSuchMethod) プロパティが廃止予定となり、近い将来削除されることとなりました。コード内でこのプロパティが使われていた場合、今後 [ウェブコンソール](https://developer.mozilla.org/docs/Tools/Web_Console) に警告が出力されます。ECMAScript 6 仕様で定義された標準の [`Proxy`](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Proxy) オブジェクトで代用可能です。

**更新**: `__noSuchMethod__` 対応は [Firefox 44 で削除されました](https://www.fxsitecompat.dev/ja/docs/2015/nosuchmethod-is-no-longer-supported/)。
