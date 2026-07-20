# Verify an official download

Do not run a ZelixLens ROBLOX Edition package unless a production release is
listed in this repository.

## 1. Download from the official release

Download `ZelixLens-ROBLOX-Edition.zip` and `SHA256SUMS.txt` from the same entry
on the [official Releases page](https://github.com/Zaroomx/ZelixLens-Roblox-Releases/releases).

Do not use copies sent through direct messages or hosted on unofficial mirrors.

## 2. Calculate the SHA-256 value

Open PowerShell in the download folder and run:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\ZelixLens-ROBLOX-Edition.zip
```

Confirm that the printed value exactly matches the value beside
`ZelixLens-ROBLOX-Edition.zip` in `SHA256SUMS.txt`.

## 3. Check the release record

An approved release also publishes:

- `update-manifest.txt` — updater asset metadata
- `update-manifest.sig` — RSA-3072 signature for that metadata
- `ZelixLens-ROBLOX-Edition.provenance.json` — release provenance
- `ZelixLens-ROBLOX-Edition-NOTICES.txt` — product and third-party notices

The launcher verifies the signed manifest, pinned GitHub URL, runtime size, and
runtime SHA-256 digest before accepting an automatic update.

## What verification means

A matching SHA-256 value confirms that the downloaded file matches the asset
published in the official release. It does not independently establish that
software is safe, compatible, permitted by Roblox, or suitable for a computer.

If values do not match, delete the download and report the mismatch privately
through the [security policy](../SECURITY.md).
