---
layout: page
title: Privacy policy
permalink: /privacy/
---


_Last updated: 21 October 2026_

This policy describes how the Atlassian Marketplace app "Undelete – Recycle Bin & Restore for Jira" (the "App") processes data. The App is provided by **Bc. Tomáš Buchta, sole trader, Company ID (IČO) 21540951, registered office 30. dubna 2307/12, 702 00 Ostrava, Czech Republic** ("we"). Contact: **[t.buchta@post.cz](mailto:t.buchta@post.cz)**.

## 1. What the App stores
To make deleted Jira issues restorable, the App stores, inside your Jira Cloud site's Atlassian Forge storage:
- copies of issue data (fields, comments, worklogs, links, attachment metadata) of the projects it protects;
- copies of attachment files, if attachment backups are enabled;
- for deleted issues, comments, worklogs and attachments: when and by which Atlassian account they were deleted and restored;
- the App's settings.

People are referenced only by their **Atlassian account ID**. The App does not store names, e-mail addresses or avatars; they are looked up from Jira when displayed.

## 2. Where the data is stored
All data is stored in Atlassian's infrastructure (Forge SQL, Forge Key-Value Store and Forge Object Store) and inherits Atlassian's data residency. The App does not send data to any server outside Atlassian, and we (the vendor) have no access to it.

## 3. Purpose and legal basis
The data is processed solely to provide the App's function – restoring deleted Jira content – on behalf of the Jira site, which acts as the controller; we act as processor (Art. 28 GDPR).

## 4. Retention
Copies of deleted issues, comments, worklogs and attachments are deleted automatically after the retention period configured by the site admin (30, 90, 180 or 365 days). Copies of issues that still exist are kept while the App is installed. When the App is uninstalled, Atlassian deletes the App's data according to its Forge data retention policy.

## 5. Personal data reporting and erasure
The App reports the account IDs it stores to Atlassian weekly via the Personal Data Reporting API and erases every reference to accounts that have been closed.

## 6. Data Processing Addendum
The [Data Processing Addendum]({{ '/dpa/' | relative_url }}) (Art. 28 GDPR) applies to all customers.

## 7. Sharing
We do not sell or share data. Sub-processor: Atlassian (hosting of the Forge platform).

## 8. Your rights
Site admins can exclude projects, change retention and uninstall the App at any time. For requests concerning personal data, contact your Jira site admin or us at [t.buchta@post.cz](mailto:t.buchta@post.cz).

## 9. Changes
We will publish changes to this policy on this page.
