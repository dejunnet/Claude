# Gear Inventory

A simple web app for tracking my camera and video equipment: what I own, what it's worth, and what's ready to shoot.

**Live site:** https://dejunnet.github.io/Claude

## Features

- Track each item's name, category, brand/model, serial number, value, quantity, and notes
- Status for every item: Ready, Checked out, Needs repair, Missing, or Retired / sold
- Running totals for item count, total value, ready gear, and gear that needs attention (retired items are left out)
- Search by name, brand, serial number, or notes
- Filter by category or status, and sort by name, category, value, or newest
- Pack check: tick off gear as it goes in the bag, then "Unpack all" after the shoot
- Export a JSON backup or a CSV, and import a backup on another device
- Works on phone and desktop, in light and dark mode

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app in one file |
| `gear-backup-from-notion.json` | My gear list exported from Notion, ready to import |

## How data is saved

The list is stored in the browser on each device. It does not sync between devices or back to Notion. To move the list or keep it safe, use **Export backup** and then **Import backup** on the other device.

The first time the app opens on a new device, it loads the gear list that came from Notion.

## Hosting

The site runs on GitHub Pages. In the repo, go to **Settings → Pages** and set the source to **Deploy from a branch → main → / (root)**. Any change to `index.html` goes live a minute or two after it's committed.
