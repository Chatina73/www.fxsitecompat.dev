---
title: "CSP ディレクティブ `frame-src` が `child-src` に置き換えられる形で廃止予定となりました"
date: "2015-11-17T14:08:00-08:00"
categories: ["dom", "privacy-security"]
tags: []
releases: ["45", "45-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1045891"
      title: "Bug 1045891 - Implement CSP 1.1 child-src directive"
aliases:
    - "/ja/docs/2015/csp-directive-frame-src-has-been-deprecated-in-favor-of-child-src/"
---
Content Security Policy (CSP) の [`frame-src`](https://developer.mozilla.org/docs/Web/Security/CSP/CSP_policy_directives#frame-src) ディレクティブが廃止予定となりました。`frame-src` は後方互換性のため一定期間残しつつ、CSP 1.1 の [`child-src`](https://developer.mozilla.org/docs/Web/Security/CSP/CSP_policy_directives#child-src) ディレクティブを代わりに使用してください。
