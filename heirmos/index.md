---
title: Heirmos Privacy Policy
---

# Heirmos Privacy Policy

_Last updated: 29 August 2026_

Heirmos is a private, local-first menstrual cycle tracking app for couples.
It is built to work entirely on your device, with an **optional** connection
to a server **you host yourself** (or that your partner hosts) for syncing
between two people. **We do not operate any server, and we never see,
collect, sell, or share your data.**

## What the app accesses, and why

| Access | Why | Where it goes |
|---|---|---|
| **Camera** | To scan a QR code when pairing your app with your own self-hosted server | Read once, locally, to decode the code — never saved or transmitted as an image |
| **Microphone / Speech recognition** | To dictate a log entry (mood, symptoms, energy) instead of typing it | Processed on-device only; never recorded to a file or sent anywhere |
| **Face ID / Touch ID / device passcode** (optional) | To lock the app behind whatever your phone already uses, if you turn on App Lock in Settings | Verified entirely by your device's own OS; Heirmos never sees or stores any biometric data |
| **Push notifications** (optional) | Period predictions, partner check-in alerts, daily logging reminders | Delivered via Apple's push service, triggered only by your own connected server — never by us |

## Your data lives on your device, encrypted

All cycle, check-in, mood, and settings data is stored in a local database
on your device, encrypted with AES-256-GCM. If you never connect the app to
a server, nothing about your cycle ever leaves your phone.

## Optional server connection

Heirmos can optionally connect to a **self-hosted Heirmos/Bloodarr server**
— one you run yourself (e.g. on your own hardware or a personal cloud VM),
identified by whatever address you enter in Settings. When connected:

- Your cycle and check-in data syncs to that server so it can be shared
  with your partner's device, the way the app is designed to be used.
- Messaging between partners, shared fridge notes, and shared supply
  tracking are all stored on that same server.
- An optional end-to-end encrypted relay mode (P-256 ECDH + AES-256-GCM)
  is available so that even the server operator cannot read partner
  messages in transit.
- An optional connection to **your own self-hosted Immich photo server**
  can pull photos to show as backgrounds — the app talks directly to
  *your* server using *your* API key; we are not involved in that
  connection and never see its contents.

We do not operate, host, or have access to any of these servers. Whoever
administers the server you connect to (often you, or your partner) controls
that data — the same way it would for any self-hosted software. We
recommend using an `https://` address for your server, since credentials
travel with every request.

## Backup & restore

You can export a full encrypted backup of your server's data at any time,
protected with a password you choose. We never see that password and
cannot recover it if it's lost.

## No tracking

There are no analytics SDKs, no advertising SDKs, and no third-party
crash-reporting or tracking services of any kind in Heirmos.

## Children

Heirmos does not collect personal information from anyone, including
children.

## Changes

If this policy ever changes, the updated version will be published at this
same address with a new date.

## Contact

Questions: email
[persieghinidev@gmail.com](mailto:persieghinidev@gmail.com), or open an
issue at
[github.com/persieghini/privacy-policies](https://github.com/persieghini/privacy-policies/issues).
