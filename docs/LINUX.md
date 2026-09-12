# DaemonCore Academy on Linux

DaemonCore Academy 8.0.3 supports x64 Ubuntu and Debian-family desktop systems through an AppImage and a Debian package. Academy lessons work offline. Live ranges require Docker Engine with Compose v2.

## AppImage

```shell
chmod +x DaemonCore-Academy-8.0.3.AppImage
sha256sum DaemonCore-Academy-8.0.3.AppImage
./DaemonCore-Academy-8.0.3.AppImage
```

## Debian package

```shell
sha256sum DaemonCore-Academy-8.0.3.deb
sudo apt install ./DaemonCore-Academy-8.0.3.deb
```

Compare the resulting hash with `SHA256SUMS-linux.txt` from the same release before running the app.

## Requirements

- x64 Ubuntu or Debian-family desktop system.
- Electron-compatible desktop session.
- Docker Engine and Compose v2 for disposable live ranges.
- GNOME Keyring or KWallet for protected FieldOps activation and operator identity.

Academy remains available without a keyring. FieldOps protected operations fail closed when secure storage is unavailable. Do not launch with `--password-store=basic`.

## Records and upgrades

The app keeps per-user records in `${XDG_CONFIG_HOME:-~/.config}/DaemonCore Academy`. This includes progress, evidence exports, and local case records. Back up important records through the in-app export controls before changing distributions or keyrings.

Installing a newer Debian package upgrades the app in place. AppImage users replace the old AppImage manually. Neither package intentionally removes the existing user data directory.

## Troubleshooting

- If a live range cannot start, run `docker version` and `docker compose version` as the same desktop account used to launch DaemonCore.
- If protected storage is unavailable, unlock GNOME Keyring or KWallet and reopen the app.
- If the AppImage will not execute, use `chmod +x` or install the Debian package. Do not use `--no-sandbox` as a workaround.
- For support, email support@daemoncore.app with the app version, distribution, and exact error. Do not include credentials or private keys.
