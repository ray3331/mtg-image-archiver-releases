# MTG Image Archiver — Official Windows Releases

This is the official binary-distribution repository for **MTG Image Archiver**, a
local-first Windows desktop utility for preserving exact Magic: The Gathering card-printing
images and creating portable PDF archives.

The application source code is proprietary and is **not** published in this repository.

## Download

[Download the latest stable Windows release](https://github.com/ray3331/mtg-image-archiver-releases/releases/latest)

On the release page, most users need only the file named:

```text
MTG-Image-Archiver-<version>-x64-setup.exe
```

The other files have specialized purposes:

| File                                                  | Purpose                                                                                                  |
| ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `MTG-Image-Archiver-<version>-x64-setup.exe`          | Windows x64 installer                                                                                    |
| `MTG-Image-Archiver-<version>-x64-setup.exe.blockmap` | Differential-update metadata used by the application                                                     |
| `latest.yml`                                          | Version, checksum, and update metadata used by the application                                           |
| `Source code (zip)` / `Source code (tar.gz)`          | GitHub-generated archives of this public documentation repository—not the proprietary application source |

Do not download the blockmap or `latest.yml` for a normal installation.

## What the application does

- Creates and reopens user-controlled, portable card-image archives.
- Resolves exact Magic printings and retrieves selected images from configured providers.
- Imports common Card List formats and exchanges exact-printing archive data.
- Creates calibrated A4, US Letter, custom-size, and duplex PDF archives.
- Keeps diagnostics local unless the user explicitly copies or exports them.
- Checks for newer public stable releases and presents their release notes before updating.

## Installation

1. Open the [latest release](https://github.com/ray3331/mtg-image-archiver-releases/releases/latest).
2. Download the Windows x64 installer.
3. Verify that it came from this repository. For stronger verification, follow
   [VERIFY_DOWNLOADS.md](VERIFY_DOWNLOADS.md).
4. Run the installer and review the Application Licence when prompted.

If Windows displays a reputation warning, confirm that the download URL belongs to
`github.com/ray3331/mtg-image-archiver-releases` and verify the SHA-256 digest before deciding
whether to continue. Do not run a copy obtained from an unrelated website.

## Updates

The application checks the same public release feed used by this page. Its update control appears
only when a newer stable version is publicly available. Draft releases are intentionally invisible
to installed applications.

## Data and privacy

Archives, downloaded images, PDF outputs, and print history are stored in locations controlled by
the user. Provider-backed features make the network requests needed for the actions the user
initiates. The exact privacy behavior for each application version is documented by the Privacy
Notice packaged with that installer.

## Support and security

- For usage help, bug reports, and improvement suggestions, read [SUPPORT.md](SUPPORT.md).
- For suspected security vulnerabilities, read [SECURITY.md](SECURITY.md) before reporting them.
- Contact: [ray.mtgarchiver@gmail.com](mailto:ray.mtgarchiver@gmail.com)

## Licence and unofficial status

MTG Image Archiver is proprietary freeware. The compiled application may be used free of charge,
and an unmodified official installer may be shared only under the terms presented by the installer
and included with the installed application. No right to the unpublished source code is granted.

MTG Image Archiver is unofficial fan-made software. Wizards of the Coast LLC and Hasbro, Inc. have
not approved, sponsored, or endorsed it. Magic: The Gathering, card names, card data, card images,
artwork, symbols, and related marks and materials belong to their respective owners. The
application must not be used to create or distribute counterfeit cards, proxy products, or other
unauthorized reproductions.

The installer includes the complete Application Licence, Distribution Notice, Privacy Notice, and
Third-Party Notices applicable to that version.
