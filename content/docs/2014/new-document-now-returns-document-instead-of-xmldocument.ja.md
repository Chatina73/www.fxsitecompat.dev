---
title: "`new Document()` が `XMLDocument` の代わりに `Document` を返すようになりました"
date: "2014-06-09T02:46:54-04:00"
categories: ["dom"]
tags: []
versions: ["32"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1017932"
      title: "Bug 1017932 – Document() constructor should return Document object (not XMLDocument)"
---
`Document` コンストラクターが、最新の仕様に従い、[`XMLDocument`](https://developer.mozilla.org/docs/Web/API/XMLDocument) の代わりに [`Document`](https://developer.mozilla.org/docs/Web/API/Document) オブジェクトを返すようになりました。これらは [`load`](https://developer.mozilla.org/docs/Web/API/XMLDocument.load) メソッドが `XMLDocument` のみで使用可能になっていることを除けば同じものです。[`DOMImplementation.createDocument`](https://developer.mozilla.org/docs/Web/API/DOMImplementation.createDocument) メソッドはこれまで通り `XMLDocument` オブジェクトを返します。
