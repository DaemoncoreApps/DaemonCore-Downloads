# DaemonCore FieldOps in Academy 10.0.0

FieldOps is included with DaemonCore Academy 10.0.0 on Windows and Linux. No FieldOps purchase, activation code, or Lemon Squeezy entitlement is required. FieldOps is a local-first assessment workspace; it does not grant permission to test a system.

## What it does

FieldOps carries an authorized engagement from preparation through evidence and reporting:

- enrolls a named operator with a device-protected Ed25519 identity;
- records the client, approving authority, authorization reference, network boundary, exact targets, exact TCP ports, and testing window;
- creates a signed engagement permit and rechecks that permit before execution;
- resolves authorized hostnames and pins operations to approved addresses;
- performs DNS, TCP reachability, port, HTTP, TLS, service-profile, web-map, and surface-baseline observations;
- runs managed Nmap through a local executable or the pinned Docker adapter when available;
- coordinates repeatable service-inventory, surface-verification, and complete-assessment campaigns;
- exports signed scope manifests for customer-controlled specialist tools and imports structured evidence without executing imported content;
- records findings, remediation, disposition, retest decisions, audit entries, and integrity results;
- supports operator-defined, explicitly authorized k6 load profiles and bounded Chaos Engine resilience exercises;
- exports printable reports and machine-readable case bundles for client retention and review.

## Authorization boundary

Every runnable operation requires a valid protected operator identity, written authorization, an active signed engagement, exact target and port membership, a valid testing window, and the selected policy and execution capacity. Changing a signed field requires a new permit. FieldOps does not provide arbitrary shell execution, unrestricted exploitation, credential spraying, payload generation, or permission to test third-party systems without written authorization.

Professional execution uses the exact target and port lists signed into the engagement. It removes product-cardinality ceilings; it does not remove scope enforcement, destination pinning, stop controls, evidence integrity, or legal responsibility. Chaos Engine is bounded resilience sampling, not a DDoS tool.

## Tool and platform notes

- Nmap and Docker are supported execution paths for the capabilities described above.
- k6 is used for managed HTTP workload profiles when it is installed locally.
- Nuclei, Locust, TShark, Hashcat, and other cataloged tools are evidence-bridge workflows: FieldOps can export signed scope and import structured results, but it does not execute imported content as a command.
- Windows uses protected operating-system credential storage.
- Linux operator identity enrollment requires an unlocked GNOME Keyring, KWallet, or another Secret Service-compatible backend. Do not run with Electron's `basic_text` password store.

## Evidence and limits

FieldOps produces tamper-evident local records, not independent identity verification or a guarantee that an operator's authorization claim is truthful. Export important case material into the client's normal evidence-retention system. FieldOps does not replace written authorization, legal review, a SIEM, EDR, vulnerability-management platform, packet-capture platform, or specialist malware and wireless tooling.

For installation and Docker/keyring troubleshooting, see [LINUX.md](LINUX.md) and the [public release guide](PUBLIC-RELEASE-GUIDE.md). For support, include the app version, platform, package type, operation name, and exact visible error; never send passwords, private keys, or unredacted customer evidence.
