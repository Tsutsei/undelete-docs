---
layout: page
title: Undelete for Confluence – user guide
permalink: /confluence/
---

Undelete – Trash Audit & Restore for Confluence shows who deleted, emptied, restored or moved which page, and restores deleted pages, blog posts and attachments to their original place – even after the trash was emptied.

## Where to find it
- **Confluence admins:** ⚙ Settings → *Undelete – Trash & Audit* (left menu, under "Apps"). Covers every space.
- **Space admins:** Space settings → Integrations → **Undelete** (if allowed in Settings). Covers that space only.

## Restoring a deleted page
1. Open **Deleted pages**, search by title or location, click **View & restore**.
2. The preview shows where the page was, who deleted it and when, its content, attachments and the child pages Confluence moved up a level when it was deleted.
3. Choose the options and click **Restore page**:
   - **Put it back in its original place** – under its original parent, before its original next sibling.
   - **Move its child pages back under it** – Confluence moves child pages to the grandparent when a page is deleted; Undelete puts them back (only those still where Confluence left them).
4. If the page is **still in the Confluence trash**, Undelete restores the same page (same ID, history, comments and attachments).
   If the **trash was emptied**, Undelete re-creates it from its copy: body, labels, attachments (from backup copies) and comments (with a note naming the original author and date). The new page has a new ID and an info panel saying when it was restored.

Tick several pages and click **Restore selected** to restore them together; parent pages are restored before their children. If another page now has the same title, the restored page is named "Title (restored)".

## Mass deletions
When one person deletes at least N pages (Settings, default 10) within 10 minutes, a yellow banner appears with **Restore all**. Optionally, Undelete creates an alert page in a chosen space that mentions the admins who ticked "Notify me", so Confluence notifies them.

## Deleted attachments
**Deleted attachments** lists files deleted from pages that still exist, whether still in the trash or already emptied (✓ backup copy kept). **Restore** puts them back on their page.

## Activity log
**Activity log** records deletions, emptied trash, restores (by Undelete or in Confluence), moves (from → to) and archiving, with who did it and when – the events Confluence's own audit log does not show. Filter by type or search by title.

## Settings
- **Excluded spaces** – no copies are kept for them.
- **Keep copies for** – how long deleted content stays restorable (30–365 days); **Keep the activity log for** 90–730 days.
- **Attachments** – keep backup copies of deleted attachments (on by default) up to a size limit (default 100 MB, max 1 GB).
- **Space administrators** can see and restore deletions in their own spaces (on by default).
- **Page index** – Undelete indexes the page tree (titles and positions only) of every space when installed; run it again if needed.

## Good to know
- Only content deleted after installation can be restored after the trash is emptied. Content still in the trash can always be restored in place.
- Undelete copies a page when it goes to the trash. If the trash is emptied within seconds, the copy may be missing – the list shows "Trash emptied – no copy".
- Comments on re-created pages are added by the app user, with the original author and date in a note.
