# WattShift Privacy Policy

_Last updated: 21 August 2026_

WattShift is a local energy cost optimizer that times high-wattage
appliance runs against your electricity tariff. It is built to work
entirely on your device: **we do not operate any servers, and we do
not collect, transmit, sell, or share any of your data. Ever.**

## What the app accesses, and why

| Access | Why | Where it goes |
|---|---|---|
| **Camera / Photo library** | To scan or pick a photo of a utility bill so the rate schedule on it can be read | Processed on-device only, then deleted — never saved to your library, and never leaves your device |
| **Notifications** | To remind you when a scheduled appliance run's cheapest window has arrived | Generated and scheduled entirely on-device by iOS/Android's own notification system — never a push notification, since there is no server to push from |

WattShift does **not** request location, microphone, or contacts
access, and has no account system, login, or biometric lock of any
kind.

Bill scanning uses on-device OCR (Google ML Kit) to read the rate
figures printed on the photo. The photo and the text extracted from it
never leave your phone, and the photo itself is deleted once the scan
is done.

## Network use

WattShift makes network requests only to fetch electricity rate data,
straight from your device to the supplier/grid-operator's own public
API — never through a server of ours, because we don't run one. Which
one it talks to depends on the region you configure in Settings:

1. **Octopus Energy or EDF Energy (UK)** — public tariff rate lookups,
   no account or key required.
2. **ENTSO-E Transparency Platform (EU)** — day-ahead prices. Requires
   a free personal API token you generate yourself at
   [transparency.entsoe.eu](https://transparency.entsoe.eu); it's sent
   directly from your device to ENTSO-E with every request and is
   never seen by us.
3. **OpenEI (US)** — utility rate lookups by ZIP code, using a free
   personal API key you generate yourself and enter in Settings.
4. **AEMO NEMWEB (Australia)** — public wholesale price data, no
   account or key required.
5. **JEPX (Japan)** — public day-ahead spot price data, no account or
   key required.

If a scanned/manually-entered bill is used instead (for a utility
with no public API), no network request is made for rates at all —
everything is calculated from what you entered, locally.

There are no analytics, no advertising SDKs, no third-party crash
reporting services, and no tracking of any kind.

## Payments

WattShift Pro is a one-time purchase — never a subscription — handled
entirely by Apple's App Store or Google Play. Your card details never
reach WattShift; the store only tells the app whether you've
purchased, and that's stored on your device like any other setting.

## Your data, your control

- Every appliance, tracked cycle, rate plan, and savings record lives
  in the app's private, sandboxed local database on your device — not
  on any server we run, because we don't run one.
- You can back up everything at any time (Settings → Backup &
  Restore), as a single file encrypted with a password only you
  choose (AES-256-GCM). We never see that password and can't recover
  it if it's lost.
- If you add the WattShift home-screen widget, only a suggested
  appliance/cycle summary is stored in a small on-device area the
  widget reads from — never a full bill, account number, or API key.
- Deleting the app deletes all app data.

## Children

WattShift does not collect personal information from anyone,
including children.

## Changes

If this policy ever changes, the updated version will be published at
this same address with a new date.

## Contact

Questions: email
[persieghinidev@gmail.com](mailto:persieghinidev@gmail.com), or open an
issue at
[github.com/persieghini/privacy-policies](https://github.com/persieghini/privacy-policies/issues).
