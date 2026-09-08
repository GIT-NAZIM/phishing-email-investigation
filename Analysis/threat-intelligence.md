# Threat Intelligence Investigation

## Indicator Investigated

Domain:

login-micr0soft-security.example

## Source

VirusTotal

## Investigation Result

The domain was searched in VirusTotal for reputation and
threat-intelligence context.

The domain is part of the synthetic investigation scenario and
uses the reserved `.example` namespace. Therefore, it should not
be treated as a real-world malicious domain or expected to have
real reputation/detection history.

## Analyst Assessment

No real-world reputation can be established for this synthetic
indicator.

However, the domain remains suspicious within the incident
scenario because:

1. It uses a Microsoft lookalike spelling (`micr0soft`).
2. It appears in a credential-verification phishing email.
3. The sender domain is consistent with the URL domain.
4. The `/verify` path supports the suspected credential-harvesting
   objective.

## Limitation

This project uses fictional infrastructure for safe portfolio
demonstration. Threat-intelligence results for the synthetic
domain must not be represented as evidence from a real phishing
campaign.