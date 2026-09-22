# Jupiter 0.1/0.2a (Alpha)

[![bluebuild build badge](https://github.com/gasterboi2012/jupiter/actions/workflows/build.yml/badge.svg)](https://github.com/gasterboi2012/jupiter/actions/workflows/build.yml)

# PLACEHOLDER (W?)

## Installation

To rebase an existing atomic Fedora installation to the latest build:

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/gasterboi2012/jupiter:latest
  ```
- Reboot to complete the rebase:
  ```
  systemctl reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/gasterboi2012/jupiter:latest
  ```
- Reboot again to complete the installation
  ```
  systemctl reboot
  ```
