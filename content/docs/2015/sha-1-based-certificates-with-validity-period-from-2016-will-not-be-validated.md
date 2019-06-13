---
title: "SHA-1-based certificates with validity period from 2016 will not be validated"
date: "2015-09-13T21:46:00-04:00"
categories: ["privacy-security"]
tags: []
versions: ["48"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=942515"
      title: "Bug 942515 - Show Untrusted Connection Error for SHA-1-based SSL certificates with notBefore >= 2016-01-01"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1254667"
      title: "Bug 1254667 - switch certificate verification SHA1 policy to \"allow for locally-installed roots\""
    - url: "https://blog.mozilla.org/security/2014/09/23/phasing-out-certificates-with-sha-1-based-signature-algorithms/"
      title: "Phasing Out Certificates with SHA-1 based Signature Algorithms"
---
The support for certificates using the [weak SHA-1 hash algorithm](https://developer.mozilla.org/docs/Web/Security/Weak_Signature_Algorithm) has been [deprecated since Firefox 36](https://www.fxsitecompat.dev/en-CA/docs/2014/sha-1-support-has-been-deprecated/). As a part of the deprecation process, SHA-1-based certificates with a period of validity beginning on or after <time datetime="2016-01-01">January 1, 2016</time> are no longer validated by Firefox 43 and later, and "[This Connection is Untrusted](https://support.mozilla.org/kb/connection-untrusted-error-message)" alert page will be displayed on sites using such a certificate.

Webmasters: Open the [Web Console](https://developer.mozilla.org/docs/Tools/Web_Console), load your site, and make sure a SHA-1-based certificate is *not* used. If the Console warns about a SHA-1-based certificate, contact the issuer to replace it with a new SHA-2-based one for free, regardless of the validity period. Firefox, among other browsers, will show the Untrusted Connection error message for all SHA-1-based certificates after <time datetime="2017-01">January 2017</time>.

**Update**: It has been reported that some Firefox users with MITM software installed on their computer are no longer able to visit any HTTPS sites due to the dynamically-generated certificates. After [some discussion](https://groups.google.com/d/topic/mozilla.dev.platform/ZNKxYgIk_Sg/discussion), this change has been [reverted with Firefox 43.0.4](https://bugzilla.mozilla.org/show_bug.cgi?id=1236975) to allow Mozilla developers to investigate the scope of this risk. See also the [Mozilla Security Blog](https://blog.mozilla.org/security/2016/01/06/man-in-the-middle-interfering-with-increased-security/).

**Update**: This restriction has been reintroduced with Firefox 48 but with an exception of locally-installed root certificates, which is intended to avoid compatibility issues with MITM software. Any SHA-1 certificates issued by a public CA after January 2016 will be rejected.

**Update** The SHA-1 support will be [disabled in January 2017](https://www.fxsitecompat.dev/en-CA/docs/2016/sha-1-certificates-issued-by-public-ca-will-no-longer-be-accepted/).
