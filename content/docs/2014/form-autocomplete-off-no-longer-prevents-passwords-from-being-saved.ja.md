---
title: "`<form autocomplete=\"off\">` がパスワードの保存を抑止しなくなりました"
date: "2014-03-21T04:50:04-04:00"
categories: ["privacy-security"]
tags: []
releases: ["30", "31-esr"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=956906"
      title: "Bug 956906 – ignore autocomplete=\"off\" when offering to save passwords via the password manager"
---
Firefox は、[`<form>`](https://developer.mozilla.org/docs/Web/HTML/Element/form) もしくは [`<input>`](https://developer.mozilla.org/docs/Web/HTML/Element/input) 要素に `autocomplete="off"` 属性を設定することで [フォームの自動補完を無効化する](https://developer.mozilla.org/docs/Web/Security/Securing_your_site/Turning_off_form_autocompletion) 手段をページ作者に提供してきました。この機能は今後「本来あるべき」挙動になります。つまり、自動補完はこれまで通り無効化できる一方で、[パスワードマネージャー](https://support.mozilla.org/kb/password-manager-remember-delete-change-passwords) はパスワード保存したいかどうか常にユーザーに尋ねるようになります。Internet Explorer と Chrome も同様の変更を行っています。
