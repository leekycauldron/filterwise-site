---
title: Filterwise support
---

# Filterwise support

Filterwise is a free early beta. YouTube changes its pages often; when it does, a page type can stop
being filtered until Filterwise is updated. Reports help fix that quickly.

**Contact:** open an issue at
[github.com/leekycauldron/filterwise-site/issues](https://github.com/leekycauldron/filterwise-site/issues).
Issues are public, so include only the details listed below and nothing personal.

## Report a video that should have been hidden

1. Open Filterwise's settings (click the Filterwise icon, then **Manage all rules**) and scroll to
   **Diagnostics**. Note the row for the page type you were on (Home, Search, Subscriptions, Watch
   page or Shorts): adapter version, last successful scan, and error count.
2. On the YouTube page, right-click the video that stayed visible and choose **Inspect**. Note the
   name of the highlighted card element (for example `ytd-rich-item-renderer` or
   `yt-lockup-view-model`) and whether it has the class `filterwise-card`.
3. Send the page type, the diagnostics row, the element name, the rule that should have matched,
   and your Chrome version (`chrome://version`).

Please **do not** send screenshots of your personal feed or watch history. The information above
contains no personal data and is enough to investigate.

## Report something hidden that should not be

Open the Filterwise popup on that page: the **This page** list shows each hidden video and the rule
that matched. Use **Reveal** to show it once, or add an **Always allow** exception in settings. If
the matching rule looks wrong, send the rule text and the video title.

## Something else broke

Turn Filterwise **Off** from its popup; everything it hid comes back immediately. Then report what
you saw, the page type, and your Chrome version.
