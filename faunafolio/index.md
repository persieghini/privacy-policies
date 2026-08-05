# FaunaFolio Privacy Policy

_Last updated: 4 August 2026_

FaunaFolio is a personal wildlife journal. It is built to work entirely
on your device: **we do not operate any servers, and we do not collect,
transmit, sell, or share any of your data. Ever.**

## What the app accesses, and why

| Access | Why | Where it goes |
|---|---|---|
| **Camera** | To photograph animals for your journal entries | Saved on your device (and to your system photo library, like a normal camera) |
| **Location (while using the app)** | To record where a sighting happened and show it on your map | Stored only in the app's local database on your device |
| **Photo library** | To import existing photos into your journal, and to save photos you take | Read/written locally; nothing leaves your device |
| **Microphone / Speech recognition** | To dictate field notes instead of typing them | Processed on-device only; never recorded to a file or sent anywhere |
| **Face ID / Touch ID / device passcode** (optional) | To lock the app behind whatever your phone already uses, only if you turn on App Lock in Settings | Verified entirely by your device's own OS; FaunaFolio never sees or stores any biometric data |

Species recognition and voice-note dictation both run **entirely
on-device** (Apple Vision / on-device Siri speech on iOS, Google ML
Kit and on-device speech recognition on Android). Your photos and your
voice are never uploaded for analysis.

## Network use

FaunaFolio makes network requests in these cases:

1. **Map tiles** — the sightings map loads imagery from
   [OpenStreetMap](https://www.openstreetmap.org). Tile requests
   necessarily reveal your map viewport to the OSM tile servers, as
   with any map app. Viewed tiles are cached on-device so previously
   seen areas work offline.
2. **Weather auto-fill** — when you log a sighting with a location,
   the app sends that coordinate and the sighting's date/time to
   [Open-Meteo](https://open-meteo.com) (a free, keyless weather API)
   to fill in the entry's weather field automatically. No account, no
   API key, and nothing else about you or the device is sent. If the
   request fails or the data isn't available yet, the field is just
   left blank — nothing else about the save is affected.
3. **City/country lookup & place search** — when you log a sighting
   with a location, the app asks your phone's own operating system to
   turn that coordinate into a city/country name (Apple's geocoder on
   iOS, Google's on Android). The same geocoder also powers "Search a
   place", available anywhere you can set a sighting's location:
   typing a place name sends that text to it to find matching
   coordinates. We don't operate this service or receive anything
   from it — it's the same lookup any map or camera app on your phone
   does — but the coordinate (or, when searching, the text you type)
   does briefly leave the device to reach it. You can turn this off
   in Settings → Geography ("Look up city/country"); sightings still
   save fine without it — an auto-filled place name just won't
   appear, and place search is unavailable — though you can always
   type a place name directly onto a sighting without it being
   looked up.
4. **Your own Immich server (optional)** — if you connect a
   self-hosted [Immich](https://immich.app) photo server, the app
   talks directly to *your* server using *your* API key. We are not
   involved in that connection and never see its contents. This
   feature is off unless you configure it. We recommend an `https://`
   server address, since your API key travels with every request; the
   app will let you use a plain `http://` address instead if your
   server doesn't have TLS set up (common for a purely local-network
   setup) — you'll see a warning when you do, since that key then
   travels unencrypted to reach it.

There are no analytics, no advertising SDKs, no third-party crash
reporting services, no tracking of any kind. If the app crashes, a
plain-text log is written to your device only — never transmitted
anywhere automatically — which you can choose to share (Profile →
Backup & restore → Share crash log) if you want to report a bug.

## Payments

FaunaFolio Pro is a one-time purchase — never a subscription — handled
entirely by Apple's App Store or Google Play. Your card details never
reach FaunaFolio; the store only tells the app whether you've
purchased, and that's stored on your device like any other setting. A
code from a friend (Settings → Redeem a code) unlocks the same thing
without any purchase at all — it's checked entirely on your device, no
server involved, no account, nothing sent anywhere.

## Your data, your control

- All journal data (entries, photos, achievements, settings) lives in
  the app's private, sandboxed storage on your device, protected by
  your device's own lock screen and storage encryption — not on any
  server we run, because we don't run one.
- You can export everything at any time (Profile → Backup & restore)
  as a portable archive, or as CSV/GPX. The full backup (which, unlike
  a single shared trip export, can include your Immich server URL and
  API key) is separately encrypted with a password you choose — we
  never see that password and can't recover it if it's lost.
- If you add the FaunaFolio home-screen widget (iOS), your streak
  count and your last sighting's name and date are stored in a small
  on-device area the widget reads from — never your photos, notes, or
  coordinates, and never off-device.
- Deleting the app deletes all app data. Photos you chose to save to
  your system photo library remain there, under your control.

## Children

FaunaFolio does not collect personal information from anyone,
including children.

## Changes

If this policy ever changes, the updated version will be published at
this same address with a new date. Since the app collects nothing,
changes are unlikely.

## Contact

Questions: email
[persieghinidev@gmail.com](mailto:persieghinidev@gmail.com), or open an
issue at
[github.com/persieghini/privacy-policies](https://github.com/persieghini/privacy-policies/issues).
