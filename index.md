---
layout: page
title: Undelete for Jira – user guide
permalink: /
---

_Looking for Confluence? See the [Undelete for Confluence guide]({{ '/confluence/' | relative_url }})._

## Where to find it
- **Jira admins:** ⚙ Settings → Apps → *Undelete – Recycle Bin* (left menu, under "Apps").
- **Project admins:** in the project, open the project tabs → **More** → *Recycle bin* (if allowed in Settings).

## Restoring a deleted issue
1. Open **Deleted issues**, search by key or summary, click **View & restore**.
2. Check the preview: fields, comments, attachments (✓ = backup copy exists).
3. Choose what to restore (comments, worklogs, attachments, links, status, sub-tasks) and click **Restore issue**.
4. The issue is re-created with a new key. Find it later with JQL: `restoredFrom = PROJ-123`.

Restore several issues at once by ticking them and clicking **Restore selected**.

## Mass deletions
When one person deletes at least N issues (Settings, default 10) within 10 minutes, a yellow banner appears with **Restore all**. Optionally, the app creates an alert issue in a chosen project and adds the admins who ticked "Notify me" as watchers, so Jira e-mails them.

## Deleted comments, worklogs and files
**Deleted comments & files** lists items deleted from issues that still exist; **Restore** puts them back (comments with a note naming the original author and date).

## Boards: change log and deleted boards
The **Boards** tab (Jira admins) shows who created, changed or deleted boards and what changed – renames, filter and its query, location, columns and their statuses, column limits and estimation.

**Deleted boards** keeps the last known configuration of each deleted board. **Details & re-create** shows it and re-creates the board with its name, type, location and filter (if the filter was deleted too, a new filter with the saved query is created). Jira doesn't let apps set columns, quick filters or swimlanes, so the dialog lists the columns and their statuses for you to set up in Board settings.

The configuration of existing boards is captured once after installation; changes are recorded from then on.

## Settings
- **Excluded projects** – no copies are kept for them.
- **Retention** – how long deleted content stays restorable (30–365 days).
- **Attachments** – keep backup copies (on by default) up to a size limit (default 100 MB, max 1 GB).
- **Back up existing issues** – run once after installation to fully protect issues that have not changed since.

## Good to know
- Only content deleted after installation can be restored.
- Comments and worklogs are re-added by the app user, with the original author and date in a note.
- Attachments above the size limit, or uploaded and deleted within a few minutes, may have no backup – the preview shows which.
