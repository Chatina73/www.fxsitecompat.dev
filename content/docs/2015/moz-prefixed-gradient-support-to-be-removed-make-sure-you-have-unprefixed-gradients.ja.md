---
title: "`-moz` 接頭辞付きグラデーション対応が廃止予定のため、接頭辞なしグラデーションを必ず用意してください"
date: "2015-08-05T00:48:18-04:00"
categories: ["css"]
tags: []
versions: ["future"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1176496"
      title: "Bug 1176496 - Drop support for -moz-prefixed gradients (-moz-linear-gradient, -moz-radial-gradient)"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1186636"
      title: "Bug 1186636 - Add pref to control legacy -moz-prefixed gradients"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1337655"
      title: "Bug 1337655 - Try disabling moz-prefixed gradient functions by default"
    - url: "https://groups.google.com/d/topic/mozilla.dev.platform/egVDMiu86m0/discussion"
      title: "Intent to unship: -moz-prefixed CSS gradient functions"
---
`-moz-linear-gradient`、`-moz-repeating-linear-gradient`、`-moz-radial-gradient`、`-moz-repeating-radial-gradient` の各関数が、[Firefox 16](https://developer.mozilla.org/Firefox/Releases/16) 以降使用可能な標準の接頭辞なし [CSS グラデーション](https://developer.mozilla.org/docs/Web/Guide/CSS/Using_CSS_gradients) に置き換えられる形で削除される方向となっています。Mozilla の開発者は Firefox 42 Nightly ビルドから一度接頭辞対応を削除しましたが、スタイルシート内で従来の接頭辞付きグラデーションのみ使われており表示が崩れるサイトが多数見つかったため、この変更はバックアウトされました。

ウェブ開発者が接頭辞付きグラデーションを無効化した状態でサイトをテストできるよう、Firefox 42 に隠し設定が追加されました。これを使うには、アドレスバーに `about:config` と入力して設定エディターを開き、`layout.css.prefixes.gradients` を検索し、この設定項目をダブルクリックして値を変更してから、あなたのサイトを読み込んであらゆる部分が問題なく表示されていることを確認します。何か問題がある場合は、接頭辞なしグラデーション、つまり [`linear-gradient`](https://developer.mozilla.org/docs/Web/CSS/linear-gradient)、[`repeating-linear-gradient`](https://developer.mozilla.org/docs/Web/CSS/repeating-linear-gradient)、[`radial-gradient()`](https://developer.mozilla.org/docs/Web/CSS/radial-gradient) あるいは [`repeating-radial-gradient`](https://developer.mozilla.org/docs/Web/CSS/repeating-radial-gradient) がスタイルシートに書かれていないということです。

影響を受けるサイトが相当数あることから、Firefox が近々この古い接頭辞対応を廃止するのは難しい状況ですが、開発者は将来にわたってサイトが使われることを考慮し、常に接頭辞なしグラデーションを使うべきです。もちろん、他の CSS プロパティ、値、関数にも同じことが当てはまります。

**更新**: [Firefox 49](https://hacks.mozilla.org/2016/09/firefox-49-fixes-sites-designed-with-webkit-in-mind-and-more/) で、未だ広く使われている `-webkit` 接頭辞付きグラデーション関数への相互運用性対応が追加されたことから、Mozilla 開発者は近々 `-moz` 対応を廃止することを検討しています。多くのサイトが `-webkit` グラデーションを使用していることを考えると、この変更のリスクは低いはずです。
