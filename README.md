# Evidex

Evidex is a command-line tool designed to capture and verify the integrity of collections of files. It produces deterministic manifests and tamper-evident audit logs so that the state of digital evidence can be verified later. The tool records the state of files at a specific moment, verifies whether those files change, and produces artifacts that can be re-verified independently in the future. The goal is not file monitoring but supporting evidence integrity and chain-of-custody workflows.

Evidex focuses on producing artifacts that remain trustworthy over time: manifests, verification reports, and tamper-evident audit logs.
The current release is a free console-based Community Edition that demonstrates the core architecture and direction of the project.

Feedback is welcome.

------------------------------------------------------------------------

## Bug Reporting and Support

The project is actively developed. Bug reports are reviewed and addressed as quickly as possible. Feature requests may or may not be implemented in the Community Edition.

For security-related reports or private communication, please use the contact information provided below.

------------------------------------------------------------------------

## Why Evidex Exists

Many tools only answer one question: Did the file change?

Evidex focuses on a broader set of questions:

-   What files existed at a specific moment
-   Whether those files changed
-   Whether the evidence artifacts themselves can still be trusted
-   How that evidence can be verified independently later

------------------------------------------------------------------------

## Key Capabilities

Community Edition currently provides:

- Deterministic file manifests
- Cryptographic file hashing (SHA-256)
- Repeatable verification of file states
- Manifest signing using RSA-SHA256
- Manifest signature verification
- Tamper-evident audit logging (hash chain)
- Audit log chain verification
- Deterministic JSON serialization (stable manifests)
- Structured verification reports
- Explicit exit codes for automation and scripting
- Clear command-line interface

Artifacts produced by Evidex can be independently verified later to confirm their integrity.

------------------------------------------------------------------------

## Project Direction

Evidex is evolving toward a broader **evidence assurance system**.

Planned directions include:

-   trusted timestamp integration
-   artifact authenticity sealing
-   chain‑of‑custody workflows
-   privacy‑aware reporting
-   high‑performance parallel hashing
-   thread‑safe async processing pipelines
-   Avalonia‑based graphical interface

The goal is to support workflows in:

-   digital forensics
-   incident response
-   compliance and audit evidence
-   regulated environments

------------------------------------------------------------------------

## Standards and Practices

The project is informed by widely used security and forensic frameworks:

-   ISO/IEC 27001 / 27002
-   ISO/IEC 27037 (digital evidence handling)
-   ISO 21043 forensic process standards
-   NIST digital evidence preservation guidance
-   GDPR privacy‑by‑design principles
-   EU trust‑service ecosystem (eIDAS)

Evidex supports workflows aligned with these practices but does not claim automatic legal compliance.

------------------------------------------------------------------------

## Editions

Community Edition

-   deterministic capture and verification
-   tamper‑evident logs
-   CLI interface
-   open documentation

Professional Edition (planned)

-   case management
-   custody workflows
-   trusted timestamp integration
-   policy packs for regulated sectors
-   advanced reporting
-   parallel processing
-   thread‑safe async processing
-   Avalonia-based graphical user interface

------------------------------------------------------------------------

## Installation

Download the latest release from the Releases section. Simply run the installer. 

------------------------------------------------------------------------

## Example Usage

Create a manifest:

    evidex scan <folder> --output manifest.json

Verify files:

    evidex verify manifest.json

Verify audit logs:

    evidex verify-audit-log audit.log

------------------------------------------------------------------------

## Documentation
-   MANUAL.md -- end‑user guide
-   docs/ -- architecture and development notes

## Star
If you like the features or the project so far, please leave a "like" by clicking the star.
Thank you.

# Contact #
- Via Github
- evidex.contact@gmail.com
