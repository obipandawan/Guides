# Welcome to SWBF

So you just landed on the server — here's everything you need to know to get going.

The short version: **join a faction immediately.** Almost everything here — credits, territory, protection — belongs to your faction, not to you individually. A lone player can survive, but a faction is how you actually compete.

---

## Table of Contents

1. [Getting Started](#1-getting-started)
2. [Your Faction's Wallet](#2-your-factions-wallet)
3. [The War for Territory](#3-the-war-for-territory)
4. [Building Safely](#4-building-safely)
5. [Useful Info Screens (LCD Panels)](#5-useful-info-screens-lcd-panels)
6. [Combat & Gear](#6-combat--gear)
7. [Tatooine — Where You're Standing](#7-tatooine--where-youre-standing)
8. [Seasons](#8-seasons)
9. [Quick-Start Checklist](#9-quick-start-checklist)

---

## 1. Getting Started

When you spawn in for the first time, you'll automatically receive a **starter kit** — no need to ask for it or run a command. It includes basic construction components, a stack of oxygen and hydrogen bottles, and a set of upgraded (Tier 3) hand tools, so you can get a foothold without immediately scavenging.

Your very next move should be joining a faction. Use the normal in-game faction menu to either join an existing one or start your own — there's a custom set of SWBF-themed faction icons to pick from when you do.

Everything from here on out — your bank account, your territory, your protection from rival builders — is tied to that faction.

---

## 2. Your Faction's Wallet

Your faction shares one pool of **Credits**. Think of it as a shared bank account, not a personal stat — everyone in the faction draws from and contributes to the same balance.

**How you get credits:** holding territory pays out automatically over time (more on that below). Admins can also set up income or bounties.

**How you spend credits:** the in-game shop sells raw material packs (ingots) in exchange for credits — useful when you need materials fast and don't have time to mine.

| Command | What it does |
|---|---|
| `/swbfe help` | List all economy commands |
| `/swbfe balance` | Check your faction's current balance |
| `/swbfe shop` | See what's for sale and the prices |
| `/swbfe buy [item]` | Buy something from the shop |

The shop sells 2,500-ingot packs of Iron, Nickel, Silicon, Cobalt, Magnesium, Silver, Gold, Platinum, and Uranium — prices scale up from Iron (cheapest) to Uranium (most expensive). Anyone in the faction can buy, not just leaders.

Check your balance often. If you're broke, the fastest way to recover is to go hold a couple of zones for a while.

---

## 3. The War for Territory

The map is dotted with capture zones — your faction earns money and standing by holding them.

### How to capture a zone

1. **Find one.** Your HUD always shows GPS pins for the 3 nearest zones. A **green pin** means you're standing inside one; **white** means it's nearby.
2. **Build a station** (a *static* grid, not a flyable ship) somewhere inside the zone.
3. **Place a Survival Kit** on that station.
4. **Hold it.** As long as no rival faction shows up, your claim builds up over time until the zone flips to your faction.
5. If another faction parks their own kit in the same zone while you're capturing, it goes **CONTESTED** — nobody makes progress until one side backs off.

### Zone defenders — nothing is a free first capture

Every zone starts out held by the **Independent Freedom Fighters**, not by nobody. The first time anyone tries to take a zone, they have to fight through whatever defenses the Freedom Fighters have stationed there before a capture can even begin.

Zones aren't defended equally. The more valuable a zone's resources or strategic position on the planet, the heavier its defenses — a backwater zone might be lightly guarded, while a zone sitting on rich resources or a key chokepoint could be a serious fight. Scout before you commit.

### Special event zones

On top of the regular capture zones, **special event zones** can pop up anywhere on the map at random. They aren't always announced ahead of time, so you won't necessarily see one coming. Event zones come with their own special rules and challenges layered on top of the usual capture fight — treat any zone behaving unusually as a sign one might be active.

### Reading the map

When you check the zone list, each one shows a status:

| Symbol | Meaning |
|---|---|
| `○` | Unclaimed — free for anyone to take |
| `●` | Owned and currently held by a faction |
| `▶` | Capture in progress, with a % complete |
| `⚡` | Contested — two+ factions fighting over it, no progress |
| `◇` | Neutral safe zone — can't be captured at all |

### Cash and points — what holding a zone actually gets you

Every zone your faction holds pays out two things at once:

- **Credits**, straight into your faction's wallet (see Section 2) — this is the income that keeps your shop runs funded.
- **War points**, which is the number that actually matters for the leaderboard. Each zone you hold earns your faction 5 points per hour while you own it.

Points accumulate continuously and are **banked permanently** — losing the zone later doesn't take the points back. The leaderboard ranks factions by total points earned over the whole war, not by how much territory you're currently holding, so a faction that held a lot of ground early can stay ahead even after losing zones. Check `/swbf scores` or throw up an `SWBF_Scores` LCD panel to see where your faction stacks up.

If your whole faction goes offline, admins may have territory-loss protection turned on so you don't lose everything while you sleep — ask in chat if you're not sure whether that's active.

---

## 4. Building Safely

Zones aren't just a scoreboard — they're also protection.

- **Unclaimed or neutral zones**: anyone can build, no restrictions.
- **Zones your faction owns**: only your faction can build there. Rivals get blocked automatically.
- **Zones a rival faction owns**: if you try to build inside their territory, your block gets deleted on the spot — but you get every component refunded immediately, so it costs you time, not materials.

The takeaway: build inside your own territory, and don't waste time building inside someone else's.

---

## 5. Useful Info Screens (LCD Panels)

A lot of live server info is available just by renaming an LCD/text panel — no programming, no commands. Stick one of these names on a screen and it'll start showing live data automatically:

| Panel Name | Shows |
|---|---|
| `SWBF_Status` | War leaderboard + zone summary |
| `SWBF_Zones` | Full zone list with current owners |
| `SWBF_MyZones` | Just the zones your faction owns |
| `SWBF_Captures` | Any capture currently in progress |
| `SWBF_Scores` | Faction leaderboard |
| `SWBF_Economy` | Your faction's credit balance and income |

A whole separate set of `LCD_` panels covers your ship and surroundings — same deal, just rename a text panel and it updates automatically:

| Panel Name | Shows |
|---|---|
| `LCD_ServerInfo` | Server name, time, player count |
| `LCD_PlayerList` | Who's currently online |
| `LCD_FactionRoster` | Your faction's members + leader, online/offline |
| `LCD_ActiveCaptures` | Zones currently being captured |
| `LCD_PlanetList` | Detected planets and distance |
| `LCD_Compass` | Heading relative to world axes |
| `LCD_StarMap` | ASCII map of the nearest planets |
| `LCD_Trajectory` | Velocity vector + travel time to nearest planet |
| `LCD_Orbit` | Orbital velocity + altitude |
| `LCD_Speed` | Current speed (m/s and km/h) |
| `LCD_Altitude` | Altitude above sea level / planet surface |
| `LCD_Weather` | O2, pressure, gravity at your location |
| `LCD_Gravity` | Gravity magnitude + direction |
| `LCD_GridHealth` | Grid integrity % |
| `LCD_Power` | Power generation vs. consumption |
| `LCD_Hydrogen` / `LCD_Oxygen` | Tank levels |
| `LCD_Thrusters` | Thruster override + thrust status |
| `LCD_Inventory` | Full grid inventory summary |
| `LCD_Inventory_Ores` / `_Ingots` / `_Components` / `_Ammo` / `_Tools` | Inventory filtered to one category |
| `LCD_Production` | All production blocks |
| `LCD_Refineries` | Refinery queue + efficiency |
| `LCD_Assemblers` | Assembler queue |
| `LCD_IceGenerators` | O2/H2 generators + ice remaining |
| `LCD_Weapons` | Weapons on the grid |
| `LCD_Turrets` | Turret status |
| `LCD_Connectors` | Connector status |
| `LCD_Doors` | Door list + open/closed |
| `LCD_Clock` | Real-time in-game clock |
| `LCD_Date` | In-game date |

You can stack a few sections onto one panel (e.g. `LCD_Power+Hydrogen+Oxygen`) and recolor them with a suffix like `_red` or `_blue` if you want to theme your base. Adding a page number (e.g. `LCD_Inventory 2`) flips to the next page if a list is too long to fit.

---

## 6. Combat & Gear

Armor on this server isn't vanilla-strength — it's been reinforced across the board, so fights take longer and base defense actually matters. Light armor in particular got a big durability boost, so don't assume a thin wall is an easy target.

If you want even tougher walls, two craftable elite armor tiers are available beyond the standard blocks:

- **Kesselite** — a solid mid-tier upgrade, built from steel plate, uranium, and ice.
- **Beskarite** — the top tier, tougher still, built with platinum instead of uranium.

Both are craftable in any assembler once you have the ingots — worth the investment for a base you actually want to defend.

---

## 7. Tatooine — Where You're Standing

The server currently runs on **Tatooine**, a desert planet with **40 capturable zones** spread across it and **2 respawn points**, so you're never too far from a fresh start after you die.

A few things to know about living here:

- **Sandstorms.** Tatooine kicks up nasty sand storms — expect reduced visibility and treat them as a hazard, not just weather. Don't get caught out in the open mid-storm if you can help it.
- **Oxygen is decent.** You won't be gasping for air everywhere, but it's not guaranteed — don't assume every spot on the planet is breathable.
- **Ice is your fuel and air supply.** There's no surface ice lying around to scoop up — you'll need **moisture capturing devices** to pull ice out of the dry air, which then feeds your O2/H2 generators for both breathable air and hydrogen fuel. Plan your base around having one running.
- **Free refill stations exist, but they're spread out.** O2/hydrogen refill stations (the `LCD_O2H2Station` signs mentioned earlier) are placed around the map for anyone to use for free — just don't expect one right around the corner. Know where the nearest one is before you head out on a long trip.

**Coming soon:** a second planet, **Mustafar**, is planned for the future. No ETA yet — for now, Tatooine is the battlefield.

---

## 8. Seasons

The galactic conquest runs in **seasons**, and each one has its own theme. While factions are out capturing territory, the season's theme drives what else is happening on the planet around you — a Death Star flyover, recurring Imperial Star Destroyer visits, a ground invasion event, or other set-piece happenings tied to that season's story. Expect the unexpected.

New season details — theme, what's changing, what's coming — get posted in Discord a couple of weeks before launch, so you've got time to adapt and prepare instead of getting caught flat-footed.

Most seasons also bring **new planets and territory** to fight over. We're adding new ground gradually as the server grows, upgrading and stabilizing things along the way so it can actually handle the expansion — the goal is to keep growing the war without breaking the experience for the people already fighting it.

---

## 9. Quick-Start Checklist

- [ ] Grab your starter kit (automatic on first spawn)
- [ ] Join or create a faction
- [ ] Check `/swbfe balance` and `/swbfe shop`
- [ ] Find your nearest zone via GPS pins and start a capture
- [ ] Build your base *inside* a zone you own — never inside someone else's
- [ ] Set up `SWBF_Status` and `SWBF_Economy` LCD panels at your base so you always know where you stand
- [ ] If you need a refill, look for an `LCD_O2H2Station` sign

Good luck out there — see you on the battlefield.
