# Portal Content Cleanup Planner

Every Portal grows a junk drawer: test maps from 2019, apps nobody opens, layers owned by people who left years ago. This planner counts what is in yours, names what can go, and puts the cleanup in order.

## What it does

Count your items by type, how old they are, how they are shared, and who owns them, and get:

- A content health score out of 100, with a verdict: Tidy, Needs a cleanup pass, or Cleanup overdue.
- Four lists: delete candidates (stale, unviewed, and shared to nobody), items to archive first, items to reassign from departed owners, and items to retag.
- The storage you get back, estimated from the share of items flagged.
- The effort in person-days, with weeks for one person and for a team of two.
- A five-phase cleanup plan and a ten-item printable checklist.

Three presets: Small organisation (300 items), Department (2,000 items), Large enterprise (10,000 items). Clear all starts from zero.

## The part most planners get wrong

Deletion means something different on each platform, and this planner says so plainly. In ArcGIS Enterprise there is no recycle bin: a deleted item is gone, and the only way back is a WebGISDR restore of the whole organisation. In ArcGIS Online, deleted items sit in the recycle bin for 14 days, but restored items come back private with no metadata. Either way, the plan archives first, confirms with the owner second, and deletes last.

## How to use it

Open `index.html` in a browser. Pick a preset or enter your own counts from the Portal: Content, My organization, filter by item type, sort by modified date. Press "Plan my cleanup". Print the plan from the button at the bottom.

No backend, no API key, no account. Nothing you enter leaves the page. The delete list is an estimate: the planner takes the smallest of the stale, no-view, and private counts, so run the item report to confirm the exact list before anything is deleted. Effort figures are planning rules from practice, not Esri numbers.

## Sources

- Esri Support: Can deleted items be recovered in ArcGIS Enterprise? Deleted items cannot be recovered; WebGISDR restore is the only way back. Enable delete protection to avoid accidental deletion.
- Esri Blog: Recycle bin, what you need to know (ArcGIS Online, June 2024). Deleted items restorable for 14 days; restored items lose metadata and sharing and come back private.
- Esri Developer: Recycle bin reference. The recycle bin is enabled by default for organisations created after the June 2024 update.

## Talk to Janaki

Questions about your own Portal? Email Janaki Gattu at gjanaki360@gmail.com with your total item count and the storage you would get back, or book a session at https://janakigattu.github.io/. She runs the cleanup with your team, or hands you the item report queries to do it yourself.
