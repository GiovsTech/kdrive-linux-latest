# kDrive Latest (for Linux AppImage)

This repository provides a **stable "latest" download URL** for [Infomaniak kDrive](https://www.infomaniak.com/en/ksuite/kdrive) Linux AppImages.

It automatically fetches the newest version from Infomaniak's JSON endpoint and makes it available via GitHub Releases under consistent filenames.

## Stable URLs (for Gear Lever)

### AMD64 (x86_64)
[AMD64](https://github.com/GiovsTech/kdrive-linux-latest/releases/download/latest/kDrive-latest-amd64.AppImage)


### ARM64
[ARM64](https://github.com/GiovsTech/kdrive-linux-latest/releases/download/latest/kDrive-latest-arm64.AppImage)


## How to Use with Gear Lever

1. Open **Gear Lever**.
2. Select your existing kDrive AppImage.
3. In the **Update Management** section, choose **Static URL**.
4. Paste the URL from above (AMD64 or ARM64 depending on your CPU).
6. Save.

Gear Lever will now automatically check for updates and notify you when a new version is available.

## How It Works

- A daily GitHub Action checks Infomaniak's update JSON.
- If a new version is detected, it downloads the AppImage and updates the `latest` release.
- The URL above always points to the newest version (GitHub's `/latest/download/` redirect).

## Why This Exists

Infomaniak's direct download links contain version numbers, which makes them unsuitable for Gear Lever's Static URL feature. This repo provides a stable endpoint.
