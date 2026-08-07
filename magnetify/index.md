# Magnetify Privacy Policy

_Last updated: 7 August 2026_

Magnetify turns your travel photos into digital fridge magnets on a
3D fridge you can turn around and look at from every side. It is
built to work entirely on your device: **we do not operate any
servers, and we do not collect, transmit, sell, or share any of your
data. Ever.**

## What the app accesses, and why

| Access | Why | Where it goes |
|---|---|---|
| **Camera / Photo library** | To photograph or pick a magnet, a custom fridge photo, or a side/top fridge photo | Processed on-device (including cropping a magnet out of its background) and saved to the app's local database on your device |
| **Microphone** | To record a voice note for a trip journal, only while you're actively recording | Saved on your device only |
| **Speech recognition** (optional, separate permission) | To transcribe a voice note live as you record it | Processed entirely on-device; the audio itself is never sent anywhere to produce the transcript |
| **Face ID / Touch ID / device passcode** (optional) | To lock the app behind whatever your phone already uses, only if you turn on App Lock in Settings | Verified entirely by your device's own OS; Magnetify never sees or stores any biometric data |

Magnetify does **not** request location permission and does not read
your device's GPS. A journal's location comes only from a place name
you type or coordinates you paste in yourself.

## Network use

Magnetify makes network requests in these cases:

1. **Place lookup (OpenStreetMap Nominatim)** — when you save a
   journal's location as text, or the app looks up a country from
   coordinates, that text/coordinates are sent to
   [Nominatim](https://nominatim.openstreetmap.org), a free geocoding
   service run by the OpenStreetMap Foundation, to find a matching
   place. No account or device identifier is attached beyond the
   location text itself. The map screen also loads map tiles directly
   from OpenStreetMap's tile servers. See the
   [OSM Foundation's privacy policy](https://osmfoundation.org/wiki/Privacy_Policy)
   for their side of this.
2. **Your own Immich server (optional)** — if you connect a
   self-hosted [Immich](https://immich.app) photo server, the app
   talks directly to *your* server using *your* API key, stored only
   in your device's secure keychain. We are not involved in that
   connection and never see its contents. This feature is off unless
   you configure it. We recommend an `https://` server address, since
   your API key travels with every request; the app will let you use
   a plain `http://` address instead if your server doesn't have TLS
   set up (common for a purely local-network setup) — you'll see a
   warning when you do, since the key then travels unencrypted to
   reach it.

There are no analytics, no advertising SDKs, no third-party crash
reporting services, and no tracking of any kind.

## Sharing

Sharing a fridge or a single magnet is always something you initiate
by tapping Share. A fridge share lets you choose, category by
category, whether to include journal notes, links, location/dates,
and voice notes — each defaults to off. Sharing a single magnet shows
you exactly what's included (notes, location, dates, voice note, if
any) in a confirmation before it's shared. Either way, the app hands
the resulting file to your device's own share sheet — you decide the
destination. Opening a fridge someone shared with you doesn't
silently become a permanent part of your own collection — you'll see
a "Save to my fridges" / "Discard" choice first.

## Payments

Magnetify Pro (unlimited fridges) is a one-time purchase — never a
subscription — handled entirely by Apple's App Store. Your card
details never reach Magnetify; the store only tells the app whether
you've purchased, and that's stored on your device like any other
setting. A redemption code from a friend unlocks the same thing
without any purchase — it's verified entirely on your device using a
cryptographic signature, with no server, no account, and nothing sent
anywhere to check it.

## Your data, your control

- Every fridge, magnet, trip journal, and voice note lives in the
  app's private, sandboxed storage on your device — not on any server
  we run, because we don't run one.
- You can back up everything at any time (Settings → Security &
  Backup), as a single file encrypted with a password only you
  choose (AES-256-GCM). We never see that password and can't recover
  it if it's lost.
- Deleting a fridge, magnet, or journal in the app deletes it (and
  its photos/voice notes) from your device immediately. Uninstalling
  the app removes everything.

## Children

Magnetify does not collect personal information from anyone,
including children.

## Changes

If this policy ever changes, the updated version will be published at
this same address with a new date.

## Contact

Questions: email
[persieghinidev@gmail.com](mailto:persieghinidev@gmail.com), or open an
issue at
[github.com/persieghini/privacy-policies](https://github.com/persieghini/privacy-policies/issues).
