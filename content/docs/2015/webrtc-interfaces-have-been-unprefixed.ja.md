---
title: "WebRTC インターフェイスの接頭辞が外れました"
date: "2015-09-25T02:46:00-04:00"
categories: ["audio-video"]
tags: []
versions: ["44", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1155923"
      title: "Bug 1155923 - Unprefix WebRTC"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1206982"
      title: "Bug 1206982 - getUserMedia spec switched from PermissionDeniedError to SecurityError"
    - url: "https://groups.google.com/d/topic/mozilla.dev.platform/V0A6ZFPYfac/discussion"
      title: "Intent to implement and ship"
---
[`RTCPeerConnection`](https://developer.mozilla.org/docs/Web/API/RTCPeerConnection)、[`RTCSessionDescription`](https://developer.mozilla.org/docs/Web/API/RTCSessionDescription)、`RTCIceCandidate` インターフェイスの接頭辞が外れました。`navigator.mozGetUserMedia` メソッドも [`navigator.mediaDevices.getUserMedia`](https://developer.mozilla.org/docs/Web/API/MediaDevices/getUserMedia) に置き換えられる形で廃止予定となりました。`moz` 接頭辞付きのインターフェイスとメソッドは近く削除されます。

また、メディア端末の使用許可設定が拒否された場合に `getUserMedia` メソッドのエラーコールバックに渡される `PermissionDeniedError` エラーコードが、最新の仕様に合わせて `SecurityError` に変更されました。
