# Verify an Official Download

Download MTG Image Archiver only from:

<https://github.com/ray3331/mtg-image-archiver-releases/releases>

Each uploaded release asset has a SHA-256 digest displayed by GitHub. A matching digest confirms
that the local file is byte-for-byte identical to the asset served by the official release page.

## Verify with PowerShell

Open PowerShell in the folder containing the installer and run:

```powershell
Get-ChildItem ".\MTG-Image-Archiver-*-x64-setup.exe" |
  Get-FileHash -Algorithm SHA256
```

Compare the complete hexadecimal hash with the `sha256:` value shown beside that installer on its
GitHub release page. Letter casing does not matter; every hexadecimal character must otherwise
match.

If the values differ:

1. Do not run the installer.
2. Delete the mismatched file.
3. Download it again directly from the official release page.
4. Report a repeated mismatch using [SECURITY.md](SECURITY.md).

## Understand the other assets

- `latest.yml` and the `.blockmap` file are automatic-update metadata. Normal users do not need
  to download them manually.
- GitHub automatically adds `Source code (zip)` and `Source code (tar.gz)` to tagged releases.
  Those archives contain this public documentation repository at the tagged commit. They do not
  contain the proprietary MTG Image Archiver application source.

Hash verification confirms file integrity relative to GitHub's hosted asset. It does not by itself
prove who authored a file or replace operating-system security controls.
