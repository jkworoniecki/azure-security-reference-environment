# Security Policy

## Scope

This repository is a public, synthetic reference implementation.

It must never contain production configurations, customer data,
credentials, access tokens, private keys, certificates, subscription IDs,
tenant IDs, internal network details, or other organization-specific
information.

## Reporting a vulnerability

Do not publish sensitive vulnerability details in a public issue.

Use GitHub's private vulnerability reporting feature if it is enabled for
this repository. Otherwise, contact the repository owner using the contact
method listed in the GitHub profile.

## Secret handling

- Do not commit secrets, tokens, private keys, certificates, connection strings, or `.env` files.
- Prefer Managed Identity and Azure RBAC for workload access.
- Treat secret scanning and push protection as secondary safeguards, not permission to commit sensitive values.
- If a secret is committed, revoke or rotate it immediately. Removing it in a later commit is not sufficient.
