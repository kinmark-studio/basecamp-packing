# 🏕 Basecamp — Crew Packing App

A smart, mobile-first packing app built for Lindsey, Chris, Lincoln & Ryder. No app store. No login. Just open in Safari and go.

## 🗂 Files

| File | What it is |
|------|------------|
| `basecamp.html` | The entire app — one self-contained file |
| `README.md` | This file |

---

## ✨ Features

### Plan Tab (✦)
A 5-step wizard that builds your packing list:

1. **Duration** — 1 night / 2–3 nights / 4–7 nights / 7–10+ nights
2. **Weather** — Warm ☀️ / Mixed 🌤 / Cold 🧊
3. **Activities** — multi-select: Ski, Raft, Bike, Camp, Hike, Beach, City, Fish
4. **Packing system** — multi-select: Carry-on, Checked bag, Backpack, Day bag, Car, Trailer, Camper
5. **Who's coming** — Lindsey, Chris, Lincoln, Ryder (all on by default)

Your answers generate a custom list — clothing quantities, gear categories, and safety items all adapt based on what you selected.

### Pack Tab (☑)
- **Person blocks** — one collapsible section per crew member, starts closed
- **Quantity badges** — scalable items (socks, underwear, base layers) show x1/x2/x3. **Tap to edit** the quantity inline
- **Check off items** — tap any item to check it, progress bar updates
- **Remove items** — tap ✕ to remove a default item you don't need
- **Restore bucket** — removed items collapse into a "↩ Removed items" bucket at the bottom of each person's section
- **Custom add** — quick-type in the field at the bottom of any section, or tap ⊕ for full options (qty + category)
- **Vault suggestions** — gear from your vault that matches your activities surfaces as a banner to review and add
- **💡 Smart suggestions** — the app learns what you add and starts suggesting it automatically on similar trips
- **Reset** — ↺ button in the list header gives surgical reset options (uncheck / remove custom / remove vault / reset crew / full reset)

### Gear Vault (◈)
Your full gear inventory — 50 items pre-loaded.

- **Filter by** activity (Raft, Bike, Hike, etc.), location (Garage, Crawl Space, Other), or person
- **View modes** — List / By Location / Grid
- **Add gear** — tap + to add a new item: icon, name, location, owner, activity tags
- **Edit/delete** — tap any item to see details, edit, or remove
- **Activity tags** — tag each item with the activities it's used for so it auto-suggests on matching trips

---

## 🧠 The Learning Engine

Every time you add a custom item to a list, the app records the trip context (activities, weather, duration, packing method). Over time:

- After **2+ trips** with the same item in similar conditions → it gets suggested
- Suggestions show as a **💡 Suggestions for you** bucket in each person's section
- Labels: *Always bring* (5+ times) / *Usually bring* (3+) / *Often bring* (high match)
- Tap **+ Add** to confirm a suggestion, or **✕** to dismiss it for 30 days

---

## 💾 Data & Storage

Everything saves automatically to **localStorage** in Safari — your gear vault, checked items, custom adds, learned suggestions, and quantity overrides all persist between sessions.

> **Important:** localStorage is tied to the browser. If you clear Safari's website data, or open the file in a different browser, you'll start fresh. Using Netlify hosting keeps everything in one stable URL.

---

## 🗄 Your Gear Vault — Pre-loaded Inventory

| Category | Items |
|----------|-------|
| Water | SUP (x2), Kids Kayak, Pack Rafts (x2), River Tubes (x2) |
| PFDs | Women's (x2), Men's (x2), Kids (x3), Dog, Women's WW Helmet, Men's WW Helmet |
| Coolers | Yeti Backpack, Canyon MD, Canyon XXL, Coleman MD |
| Fishing | Rods (x2), Tackle Box, Fly Rod, Net, Backpack |
| Packs | Hiking (x2), CamelBak 3L (x2), CamelBak 1L |
| Coffee | Aeropress (x2), Grinder |
| Camp | Blankets (x2), Neso Shade + Stakes, LG Chairs (x4), Foldable (x2), Kids Chair |
| Dog | Portable Crate |
| Bikes | Ebike, Men's MTB, Women's MTB, Kids MTB |
| Kids bike kit | Shoes, Helmet, Gloves, Glasses |
| Women's bike kit | Shoes, Helmet, Gloves, Glasses, Shorts, Shirt, Underwear |
| Men's bike kit | Shoes, Helmet, Gloves, Glasses |

Storage locations are pre-filled as **Garage** for most items — tap any item in the vault to update the location to Crawl Space or Other.

---

## 🔧 Updating the App

When new features are added, you'll get a new `basecamp.html` file. To update:

**If using Add to Home Screen from a file:**
- Delete the old shortcut, AirDrop the new file, re-add to home screen
- Note: your learned suggestions and custom qty overrides live in localStorage, not the file — they'll reset on a fresh install

**If using Netlify:**
- Go to your Netlify site dashboard → Deploys → drag the new file to re-deploy
- Your URL stays the same, localStorage persists ✓

---

## 🚧 Coming Next
- Lincoln's bag view — isolated pull of just his stuff
- Print / share — export a list as a clean checklist
- "Who's on this trip" memory — save past trip configurations

---

*Built by Claude for Lindsey, Chris, Lincoln & Ryder — Edwards, CO*
