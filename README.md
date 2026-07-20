<div align="center">

# ZelixLens ROBLOX Edition

**Official customer releases for the private ZelixLens ROBLOX Edition Windows project.**

[![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011%20x64-0078D4?style=for-the-badge&logo=windows&logoColor=white)](#system-requirements)
[![Source](https://img.shields.io/badge/Distribution-Binary%20Only-111827?style=for-the-badge)](#repository-boundary)
[![Discord](https://img.shields.io/badge/Discord-ZelixLens-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/KaA3YBZ43D)

> [!IMPORTANT]
> The first production binary release is pending code-signing and installation
> review. Do not download ZelixLens executables from direct messages, mirrors,
> or repositories other than this one.

</div>

## Repository boundary

This is the separate, public, customer-facing release repository. It contains
documentation and GitHub Release assets only.

The private source repository remains private and is not mirrored here. This
Git tree must never contain source code, build caches, signing private keys,
KeyAuth Seller keys, API secrets, customer access keys, or local credentials.

## Product overview

ZelixLens ROBLOX Edition is a separate Windows application with a D3D11 overlay,
configurable player visuals, aiming controls, and Roblox-specific compatibility
logic. Customer access is verified through KeyAuth.

Customers are responsible for complying with Roblox rules, applicable law, and
the rules of each experience they join. Use of third-party software can result
in account or platform action.

## Launcher and updates

The customer launcher is named `ZelixLens.ROBLOX.Launcher.exe`. Before launch it:

- retrieves update metadata from this repository's latest GitHub Release;
- verifies an independently signed RSA-3072 manifest;
- validates the pinned release URL, runtime size, and SHA-256 digest;
- blocks rollback and same-version asset replacement; and
- starts the runtime with a short-lived, one-use launch grant; the runtime then
  completes KeyAuth verification before loading its privileged backend.

After a key is accepted, it is saved with Windows DPAPI for the current Windows
account. The launcher can reuse that protected key on later starts, and the
**FORGET** button removes it.

The update signing private key is not stored on GitHub or shipped to customers.

## Download status

There is currently no approved production binary release. When one is ready,
the complete package and verification files will appear on the
[GitHub Releases page](https://github.com/Zaroomx/ZelixLens-Roblox-Releases/releases).

An official release will include:

- `ZelixLens-ROBLOX-Edition.zip`
- `SystemHost.exe` for authenticated runtime updates
- `update-manifest.txt` and `update-manifest.sig`
- `SHA256SUMS.txt`
- `ZelixLens-ROBLOX-Edition.provenance.json`
- `ZelixLens-ROBLOX-Edition-NOTICES.txt`

Follow [Verify an official download](.github/docs/VERIFY.md) before running a
published package.

## System requirements

- Windows 10 or Windows 11, x64
- Roblox Player
- an active ZelixLens ROBLOX Edition access key
- network access for KeyAuth verification and authenticated updates
- any separately documented, trusted system prerequisite required by the release

## Support

- [Official ZelixLens Discord](https://discord.gg/KaA3YBZ43D) for access and private support
- [Support guide](.github/SUPPORT.md) for safe diagnostic information
- [Security policy](.github/SECURITY.md) for private vulnerability reporting
- [Privacy notice](.github/docs/PRIVACY.md) for customer data flows

Never post access keys, tokens, passwords, payment information, or private
account details in a public issue or discussion.

## License

ZelixLens is proprietary, binary-distributed software. An active access license
grants only the limited right described in [LICENSE.md](LICENSE.md). Third-party
components remain subject to the notices supplied with each release.

<div align="center">

**ZelixLens ROBLOX Edition · Official customer release repository by Zaroomx**

</div>
