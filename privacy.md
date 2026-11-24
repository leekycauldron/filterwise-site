---
title: Filterwise privacy policy
---

# Filterwise privacy policy

_Effective for version 0.1.0 (early beta). Last updated 2026-11-24._

Filterwise ("the extension") hides YouTube videos that match rules you create. It is designed to
work entirely on your device. Filterwise is an independent project and is **not affiliated with,
endorsed by, or sponsored by YouTube or Google**. "YouTube" is a trademark of Google LLC and is
used here only to describe what the extension works with.

## Summary

- No account, no servers, no analytics, no advertising, no remote code.
- Rules are evaluated on your device. Filterwise itself sends nothing anywhere.
- Your rules are copied to your Google account **only if you turn on "Sync rules with Chrome
  Sync"**, using Chrome's built-in sync.

## What Filterwise reads

On YouTube pages (`https://www.youtube.com/*`) only, Filterwise reads the text shown on video cards
(titles, channel names, channel handles and channel IDs in links) so it can compare them with your
rules and hide matching cards. This happens inside your browser. Filterwise does not read pages on
any other website.

## What Filterwise stores on your device (`chrome.storage.local`)

| Data | Purpose |
| --- | --- |
| Your rules and settings | Apply your filters. |
| Per-rule match counts and last-match time | Show how often each rule hides something. |
| Up to 5 automatic backups of your rules | Recover from imports, restores, updates, repairs and synced changes. |
| One "undo" snapshot of your rules | Undo your most recent change. |
| Diagnostics per YouTube page type (adapter version, counts of cards checked/hidden/skipped, last successful scan time, last error message) | Show whether filtering is working on each page type. Contains no video titles or channel names. |

The list of videos hidden on the page you are viewing ("session activity") is kept in memory for
that tab only and is discarded when the tab closes. Filterwise does not record your watch history.

## What leaves your device

- **Nothing**, unless you turn on **Sync rules with Chrome Sync** in Filterwise's settings (off by
  default).
- With sync on, Chrome Sync stores a copy of your **rules** (keyword and phrase text, channel names,
  handles and IDs, rule type, on/off state, expiry and creation times) and your **"show
  placeholders" setting** in your Google account so they are available in Chrome on your other
  signed-in devices. Google transfers and stores this data as part of Chrome Sync. Match counts,
  session activity, diagnostics, backups, the undo snapshot, and the master on/off switch are never
  synced.

Filterwise does not sell, rent, or share data with anyone, does not use data for advertising,
creditworthiness or any purpose unrelated to filtering, and does not allow humans to read your data.

## Permissions

| Permission | Why it is needed |
| --- | --- |
| `storage` | Save your rules, settings, counts and backups on your device (and in Chrome Sync only if you turn it on). |
| Access to `https://www.youtube.com/*` | Read video cards on YouTube and hide the ones that match your rules. No other website. |

## Your choices

- Turn Filterwise off at any time from its popup; hidden videos reappear immediately.
- Edit or delete any rule, export your rules as a readable JSON file, import them elsewhere, or
  restore a backup from the settings page.
- Turn off **Sync rules with Chrome Sync** in Filterwise's settings to stop syncing. Doing so also
  deletes Filterwise's synced copy of your rules from your Google account; rules on your device stay.
- Uninstalling Filterwise deletes all of its data stored on your device.

## Changes

If this policy changes, the new version will be published at the same address with a new "Last
updated" date before the change takes effect.

## Contact

See the [support page](support.md) for how to report a problem or ask a question, or open an issue
at [github.com/leekycauldron/filterwise-site/issues](https://github.com/leekycauldron/filterwise-site/issues).
