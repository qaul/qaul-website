---
title: 'qaul 2.0.0 beta 18 released'
description: 'download & test'
date: 2024-04-11
---

# qaul 2.0.0-beta.18 released

This release moves away from the unmaintained `sled-extensions` data base extensions to a direct use of the `sled` data base.

## Changes

Added

- Automatically generate SBOM files for all binaries.
- UI redesign for simple adding of static links (Community Nodes) with many options: QUIC/TCP/IPv4/IPv6

Fixed

- UI: block user issue fixed
- UI: Network view upgraded & fixed not showing all connections
- Fixed a crash on Android, when BLE failed to initialize on a device (thanks to @link2xt)

Changed

- migrated from sled 0.29 used by sled-extensions to current sled 0.34.7.
- upgraded many libraries
- made `quic` the default transport option for static links

## Download & Test

[Download qaul App &gt;&gt;](/#download){{<br>}}
[All files of this release are available on our github page &gt;&gt;](https://github.com/qaul/qaul.net/releases/tag/v2.0.0-beta.18)

Tell us your findings via the [github issues & discussions](https://github.com/qaul/qaul.net/issues), in our [our matrix chat room `#qaul.net:c-base.org`](https://matrix.to/#/#qaul.net:c-base.org) or simply write us an [contact@qaul.net](mailto:contact@qaul.net).

For security related issues please do not file a public issue on GitHub. Instead, please [file a private security vulnerability report](https://github.com/qaul/qaul.net/security/advisories/new), or write an email to [security@qaul.net](mailto:security@qaul.net).
