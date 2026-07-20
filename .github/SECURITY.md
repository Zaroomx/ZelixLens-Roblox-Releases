# Security policy

## Official distribution

Trust a binary only when it is attached to a published release in this exact
repository: `Zaroomx/ZelixLens-Roblox-Releases`. Do not trust executables sent
through direct messages or hosted on unofficial mirrors.

Each approved release includes SHA-256 checksums, authenticated updater metadata,
a provenance record, and consolidated license notices. Follow
[the download-verification guide](docs/VERIFY.md).

## Report a vulnerability privately

Use this repository's **Security → Report a vulnerability** option to report:

- suspected release-asset tampering
- signature or checksum verification failures
- updater or launcher security defects
- leaked credentials or access-control weaknesses
- accidental exposure of private customer information

Include the affected version, a concise reproduction, expected behavior, and
observed behavior. Do not include live keys, passwords, tokens, recovery codes,
or unnecessary personal information.

If GitHub private vulnerability reporting is unavailable, open a private ticket
in the [official ZelixLens Discord](https://discord.gg/KaA3YBZ43D) and request
the security-reporting contact.

## Security-software reports

If security software flags a download, stop and verify its source and published
SHA-256 value. Do not disable operating-system security controls or create broad
security exclusions to force an unverified binary to run.
