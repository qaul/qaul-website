---
title: 'qaul 2.0.0 rc1 released'
description: 'download & test'
date: 2024-06-08
---

# qaul 2.0.0-rc.1 released

This release can only be upgraded from qaul version `2.0.0-beta.18`.
Please upgrade to beta 18 first, before upgrading to `Release Candidate 1` or later.

## Changes

Added

- Warning when trying to upgrade to this version on earlier instances of qaul 2.0.0-beta.17 and lower.
- About screen, with version information

Fixed

- Fixed a possible panic in libqaul that could occur when receiving an empty data package when receiving a file.
- Fixed UI flickering in 'Network View'.

Changed

- Upgraded libp2p to current version 0.53.2.
- Libqaul's communication protocols now have an own codec to encode and decode all messages.
  This codec is fully compatible to how qaul was sending it's messages before.
- Upgraded many libraries to new versions.
- removed old versions of unmaintained `sled` versions, which were only used for the upgrade procedure to qaul 2.0.0 beta 18.
  This means that upgrading to qaul version 2.0.0 release candidate 1 is only possible from qaul version 2.0.0 beta 18.
- Configuration auto-upgrade of all static TCP peer entries to use the QUIC protocol for interconnections.

## Download & Test

[Download qaul App &gt;&gt;](/#download){{<br>}}
[All files of this release are available on our github page &gt;&gt;](https://github.com/qaul/qaul.net/releases/tag/v2.0.0-rc.1)

Tell us your findings via the [github issues & discussions](https://github.com/qaul/qaul.net/issues), in our [our matrix chat room `#qaul.net:c-base.org`](https://matrix.to/#/#qaul.net:c-base.org) or simply write us an [contact@qaul.net](mailto:contact@qaul.net).

For security related issues please do not file a public issue on GitHub. Instead, please [file a private security vulnerability report](https://github.com/qaul/qaul.net/security/advisories/new), or write an email to [security@qaul.net](mailto:security@qaul.net).
