# DaemonCore Academy 9.0.4 public release guide

This is the customer-facing installation and support path for DaemonCore Academy 9.0.4. The official Windows edition is a $39 one-time Microsoft Store purchase with ongoing Academy content updates. Linux packages remain free. FieldOps is included with Academy; Cloud Classroom educator services remain separate.

## Choose an install channel

### Microsoft Store (recommended Windows path)

Install **Daemoncore Academy - Cyber Security** from the [Microsoft Store listing](https://apps.microsoft.com/detail/9nh4p6jbs174?hl=en-US&gl=US). Store updates and package signing are handled by Microsoft.

### Standalone Windows installer

Use the [Microsoft Store listing](https://apps.microsoft.com/detail/9nh4p6jbs174?hl=en-US&gl=US) for the official signed Windows package. Linux customers should use the public [DaemonCore Downloads release](https://github.com/DaemoncoreApps/DaemonCore-Downloads/releases/latest), which contains the AppImage, Debian package, checksums, support matrix, and installation guide.

The current standalone installer is unsigned. Verify the checksum before running it and evaluate it in a disposable Windows 10/11 VM until an Authenticode-signed installer is published.

```powershell
(Get-FileHash .\DaemonCore-Academy-Setup.exe -Algorithm SHA256).Hash
```

Only continue when the output exactly matches the value for `DaemonCore-Academy-Setup.exe` in `SHA256SUMS-windows.txt`.

### Linux

Linux packages are a separate free release asset set. Use an AppImage or Debian package only when that exact version is attached to the public release and its SHA-256 entry is present. Do not guess a download URL for a package that is not listed on the release page.

## First launch

1. Start DaemonCore Academy and complete the local operator setup.
2. Use Academy, Mission OS, Web Forge, Enterprise Forge, and non-classroom features offline after installation.
3. Docker-backed ranges require a working Docker Engine with Linux containers. The browser preview cannot start local ranges.
4. Cloud Classroom is an optional online educator service. FieldOps is included locally and requires a protected operator identity before operations can run; the local Academy remains usable without network access.

## Cloud Classroom

Cloud Classroom is the paid, online instructor/student workspace. An instructor creates an institution and cohort, generates a room enrollment code, publishes assignments, and reviews student submissions. Students create their own account, enter the instructor’s room code, and complete only the work assigned to their cohort.

The classroom sync uses Supabase Auth and row-level security. A network failure or expired session should be reported in the UI; retry after signing in again. Never paste a service-role key into the app or a browser.

## Support evidence

When reporting a problem, include:

- the exact app version shown in the footer;
- the install channel (Store or standalone);
- operating system and architecture;
- whether Docker was required;
- the visible error text and the time it occurred.

Do not include passwords, Supabase keys, private student records, or unredacted assessment evidence in a public issue.

## What 9.0.4 does not claim

- The certification page is a readiness preview, not a live credential issuer.
- Testing Mode is local assessment practice, not remote proctoring.
- Range commands run against sealed, authorized fixtures and internal services; they are not permission to test an external target.
