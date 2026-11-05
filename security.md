---
layout: page
title: Security policy
permalink: /security/
---

_Last updated: 5 November 2026_

This policy applies to the Atlassian Marketplace apps **Undelete – Recycle Bin & Restore for Jira** and **Undelete – Trash Audit & Restore for Confluence** (the "Apps"), provided by **Bc. Tomáš Buchta, sole trader, Company ID (IČO) 21540951, Ostrava, Czech Republic** ("we").

## Reporting a vulnerability
Send security issues to **[security@tsutsei-support.atlassian.net](mailto:security@tsutsei-support.atlassian.net)**. Every message creates a tracked request in our support system. Please include the app, your site URL, steps to reproduce and the impact you expect. Do not include passwords, API tokens or customer data.

We confirm receipt within 2 business days, keep you informed about the fix and credit you in the release notes if you wish. Please give us reasonable time to release a fix before disclosing the issue publicly.

## Architecture
- The Apps run entirely on **Atlassian Forge** ("Runs on Atlassian"): Forge functions, Forge storage (SQL, key-value store, object store) and UI Kit. No Forge Remote, no egress to external servers, no vendor-side servers or copies of customer data.
- Customer data stays in each customer's Forge storage, encrypted at rest and in transit by Atlassian. People are referenced by Atlassian account IDs only.
- The Apps request only the scopes their features need and never ask for passwords or API tokens.
- The Apps do not use AI or machine-learning models, and no customer data is processed by such models.

## Secure development
- Every backend call re-checks the calling user's Jira or Confluence permissions before data is read or changed.
- User input is validated against fixed choices or range-checked; database queries use bound parameters; the UI uses Atlassian UI Kit components only.
- Logs contain IDs, counts and error messages only, never content of issues or pages. Access to logs is limited to the developer (Forge developer console) and, for the Apps' activity logs, to site and project/space admins.
- Every change passes automated unit and end-to-end tests (including permission checks) before it is deployed to production.
- Dependencies are checked with `npm audit` before every release; known vulnerabilities are fixed before deploying.

## Access control
- Source code is in private GitHub repositories; GitHub and Atlassian accounts are protected with two-factor authentication.
- The developer workstation uses full-disk encryption, automatic operating system and security updates, a firewall and malware protection. Unsupported operating system versions are not used.
- Access to source code, the Forge developer console, the Marketplace partner account and the support site is reviewed every quarter.

## Fixing vulnerabilities
Vulnerabilities are scored with CVSS and fixed within the deadlines of the Atlassian Marketplace security bug fix policy:

| Severity | CVSS | Fix released within |
|---|---|---|
| Critical | 9.0 – 10.0 | 10 days |
| High | 7.0 – 8.9 | 4 weeks |
| Medium | 4.0 – 6.9 | 12 weeks |
| Low | 0.1 – 3.9 | 25 weeks |

Forge deployments reach all installations within minutes, so customers do not need to update the Apps.

## Security incidents
If a security incident may affect customer data, we report it to Atlassian within 24 hours and notify the admins of affected sites within 72 hours where possible. As a data processor under the GDPR, we inform controllers without undue delay. See also the privacy policies for [Jira]({{ '/privacy/' | relative_url }}) and [Confluence]({{ '/confluence/privacy/' | relative_url }}) and the [Data Processing Addendum]({{ '/dpa/' | relative_url }}).
