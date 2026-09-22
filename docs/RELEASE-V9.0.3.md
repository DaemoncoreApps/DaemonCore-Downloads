# DaemonCore Academy 9.0.3

DaemonCore Academy 9.0.3 is the current supported Linux release for x64 Ubuntu and Debian-family desktops. Linux packages remain free; the Windows edition is distributed through the official Microsoft Store.

## Linux package update

- AppImage and Debian packages are built from the same 9.0.3 source tree as the Windows release.
- SHA-256 checksums and the tested Linux support matrix ship with this release.
- Academy lessons, progress records, evidence exports, and local ranges remain available offline.
- Live ranges require Docker Engine with Compose v2 and a working desktop session.
- FieldOps protected operations require an unlocked GNOME Keyring or KWallet backend.

## Curriculum and platform

- CORE 01 now includes Foundation, Practitioner, and Advanced instruction with concept briefings, mental models, worked decisions, practical mechanics, retrieval checkpoints, and debriefs.
- The Academy contains 127 lessons across 505 guided sections and approximately 125 hours of instruction.
- The release validates 150 student-facing sealed scenarios across 18 specialist tracks.
- Academy and standalone FieldOps use separate application identities and protected data vaults.

## Verification

Before launch, compare the downloaded AppImage or Debian package with `SHA256SUMS-linux.txt` from this release. Use the [Linux support guide](LINUX.md) for installation, Docker, keyring, upgrade, and troubleshooting instructions.

The public Downloads repository contains release installers, checksums, support matrices, and documentation only. The application source repository remains private.

## Documentation

The complete PDF and editable Word guide set is available in the [v9.0.3 documentation directory](releases/v9.0.3/README.md).
