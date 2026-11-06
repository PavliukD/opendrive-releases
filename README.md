# OpenDrive installers

Official release packages for OpenDrive, a OneDrive Files On-Demand client for Linux.

[Download the latest release](https://github.com/PavliukD/opendrive-releases/releases/latest)

- Linux Mint 22.3 Xfce (amd64): `opendrive_VERSION_linuxmint22.3_amd64.deb`
- Ubuntu 26.04 LTS (amd64): `opendrive_VERSION_ubuntu26.04_amd64.deb`

Download the matching package and `SHA256SUMS` from the same release. Verify with `sha256sum -c SHA256SUMS --ignore-missing`, then install using `sudo apt install ./opendrive_VERSION_PLATFORM_amd64.deb`.

Starting with 0.6.0, an installed system timer checks this repository for stable releases every 15–17 minutes. It verifies the package and waits until active clients have no open files or unsynchronized changes before installing and restarting them. Clients older than 0.6.0 require one manual upgrade first.

Update status: `opendrive updates`. Disable automatic updates: `sudo systemctl disable --now opendrive-update.timer`.

This repository contains release installers, checksums and user documentation. Development source remains in a separate private repository. OpenDrive is not affiliated with Microsoft.
