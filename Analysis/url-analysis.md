# Phishing URL Analysis

## Extracted URL

hxxps://login-micr0soft-security[.]example/verify

## URL Components

| Component | Observation |
|---|---|
| Protocol | HTTPS |
| Domain | login-micr0soft-security.example |
| Path | /verify |
| Defanged | Yes |

## Findings

- The domain uses a lookalike spelling of "Microsoft".
- The domain is consistent with the suspicious sender domain.
- The `/verify` path supports the email's credential-verification theme.
- The URL is treated as suspicious and was not visited directly.
- The URL has been defanged to prevent accidental access.

## Preliminary Assessment

The URL is consistent with a credential-phishing campaign and
requires further threat-intelligence analysis.