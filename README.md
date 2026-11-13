# SBAModding release repository

This repository holds no code. Its [releases](../../releases) hold the files of mods that are **closed source or all
rights reserved**, for mods whose creators allow the project to host them. The audited mod list itself lives in the
[mod repository](https://github.com/SBAModding/ModRepository).

## How it is used

- A mod is audited first. After the review, a maintainer uploads **the exact file that was audited** as an asset of a
  new release here.
- The mod's entry in the mod repository points at that asset and pins its SHA-256 and size. SBAModLoader downloads the
  file and installs it only if both match, so a file that changes after the audit is rejected.
- Open source mods do not belong here: they are loaded from their own GitHub releases.

## Conventions

| | |
|---|---|
| Tag and release name | `<mod id>-<version>`, for example `mini-map-2.1.0` |
| Asset | one file per release, named as the mod ships it |
| Download URL | `https://github.com/SBAModding/ReleaseRepository/releases/download/<mod id>-<version>/<file>` |

Releases are never edited after they are published. A new version is a new release.

## Rights

Files are only published here with their creator's permission. Everything stays under the creator's own terms
(for example "All rights reserved"); being downloadable from this repository does not grant any license. If you are a
creator and want a file removed, open an issue.
