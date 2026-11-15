---
title: Privacy policy
---

# AS Authenticator privacy policy

Effective 14 November 2026

AS Authenticator, by Ayala Solutions, generates two-factor authentication codes on your Mac, iPhone and iPad.

## What the app stores

The secrets you add, their names, sites and categories, and your settings. They are kept on your device in a vault encrypted with AES-256-GCM under a key derived from your master password with Argon2id. If you turn on biometric unlock, a copy of the master password is wrapped by a key in the device's Secure Enclave and stored in the device Keychain. Exported vault files are encrypted the same way.

## What the app sends

Nothing, unless you turn on one of two optional features in Settings, each described there:

- **Check the clock** asks timeapi.io for the current time about once an hour so codes stay correct when the device clock drifts. The request carries your IP address and nothing else.
- **Site icons from the web** (on by default; turn it off in Settings to stop and delete the cached icons) asks a site you have an account with for its icon, once, over HTTPS, without cookies or referrer. If that host serves no icon, the same request goes once to the organisation's main domain. That site learns that a device at your IP address asked for its icon.

The app has no account system, no analytics, no advertising, no crash reporting and no tracking.

## Syncing between your devices (optional)

Off by default. If you turn on **Sync between devices** in Settings, the encrypted vault is copied through your own iCloud account to your other devices running the app, by the method you choose: iCloud Drive, iCloud Keychain or iCloud (CloudKit). What is stored in iCloud is the same AES-256-GCM-encrypted vault, plus a revision number, a timestamp and a device tag such as "iPhone-3f9a2c1b" (not your device name). Your master password never leaves the device, so Apple holds only ciphertext. iCloud Keychain data is end-to-end encrypted by Apple; iCloud Drive and CloudKit data is end-to-end encrypted only when Advanced Data Protection is on for your Apple Account, and otherwise the vault's own encryption is what protects your secrets. Sync is not available for a vault without a master password. Ayala Solutions never receives any of it.

## What we receive

Nothing. Ayala Solutions runs no server for this app and cannot see your vault, your secrets or your usage.

## Deleting your data

Settings > Delete everything removes the vault, backups, caches and Keychain items from the device. Deleting the app removes everything except the Keychain items, which Delete everything clears first. Settings > Remove synced copies from iCloud turns sync off and deletes the vault copy from iCloud Drive, iCloud Keychain and CloudKit.

## Children

The app is not directed at children under 13 and collects no information from anyone.

## Changes

If this policy changes, the new version is published at https://hov172.github.io/as-authenticator-vault/privacy with a new effective date.

## Contact

Ayala Solutions, ayala.solutions@gmail.com
