# Privacy notice

This notice summarizes the intended data flows for ZelixLens ROBLOX Edition.
It must be reviewed whenever authentication, updates, analytics, or support
behavior changes.

## License verification

The launcher uses KeyAuth. A verification request may include:

- the access key entered by the customer
- a device or hardware identifier used for license binding
- the application name and protocol version
- standard network metadata such as IP address and request time

KeyAuth processes this information under its own terms and policies.

## Local storage

- A saved access key is protected with Windows current-user encryption (DPAPI).
- A one-use launch grant passes only a short-lived random nonce to the runtime.
- Signed update proof and rollback state are protected in the current-user profile.
- Application preferences remain local unless the customer chooses to share them.

## Updates and downloads

The launcher contacts GitHub to retrieve signed release metadata and approved
runtime assets. GitHub may process normal connection and download metadata.

## Support

Discord is used for access and private support. Never submit passwords, recovery
codes, payment-card information, or unrelated personal information in a support
request, and never post an access key publicly.
