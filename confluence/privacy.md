---
layout: page
title: Privacy policy – Undelete for Confluence
permalink: /confluence/privacy/
---

_Last updated: 23 October 2026_

This policy describes how the Atlassian Marketplace app "Undelete – Trash Audit & Restore for Confluence" (the "App") processes data. The App is provided by **Bc. Tomáš Buchta, sole trader, Company ID (IČO) 21540951, registered office 30. dubna 2307/12, 702 00 Ostrava, Czech Republic** ("we"). Contact: **[t.buchta@post.cz](mailto:t.buchta@post.cz)**.

## 1. What the App stores
To show who deleted or moved content and to make deleted content restorable, the App stores, inside your Confluence Cloud site's Atlassian Forge storage:
- an index of the page tree of the spaces it protects: page and blog post IDs, titles, parent pages and positions (no page content);
- for pages and blog posts moved to the trash: a copy of their content (body, labels, footer comments, attachment list), their original location, and when and by which Atlassian account they were deleted, emptied from the trash and restored;
- copies of attachment files of deleted content, if attachment backups are enabled;
- an activity log of deletions, restores, moves and archiving (what, when, by which account);
- the App's settings.

People are referenced only by their **Atlassian account ID** (including accounts mentioned in copied content). The App does not store names, e-mail addresses or avatars; they are looked up from Confluence when displayed.

## 2. Where the data is stored
All data is stored in Atlassian's infrastructure (Forge SQL, Forge Key-Value Store and Forge Object Store) and inherits Atlassian's data residency. The App does not send data to any server outside Atlassian, and we (the vendor) have no access to it.

## 3. Purpose and legal basis
The data is processed solely to provide the App's function – auditing and restoring deleted Confluence content – on behalf of the Confluence site, which acts as the controller; we act as processor (Art. 28 GDPR).

## 4. Retention
Copies of deleted content and attachments are deleted automatically after the retention period configured by the site admin (30, 90, 180 or 365 days); the activity log after 90, 180, 365 or 730 days. When the App is uninstalled, Atlassian deletes the App's data according to its Forge data retention policy.

## 5. Personal data reporting and erasure
The App reports the account IDs it stores to Atlassian weekly via the Personal Data Reporting API and erases every reference to accounts that have been closed.

## 6. Data Processing Addendum
The [Data Processing Addendum]({{ '/confluence/dpa/' | relative_url }}) (Art. 28 GDPR) applies to all customers.

## 7. Sharing
We do not sell or share data. Sub-processor: Atlassian (hosting of the Forge platform).

## 8. Your rights
Site admins can exclude spaces, change retention and uninstall the App at any time. For requests concerning personal data, contact your Confluence site admin or us at [t.buchta@post.cz](mailto:t.buchta@post.cz).

## 9. Changes
We will publish changes to this policy on this page.
