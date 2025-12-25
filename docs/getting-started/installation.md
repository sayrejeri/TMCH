# Installation

In **Total Miner Forge**, “installation” does not mean downloading mods or configuring files.  
It refers to the **initial setup of a world** so that permissions, Creative Mode, and scripting work correctly.

This page walks through the recommended setup process before you begin building or scripting.

---

## What this page is for

This guide helps you:
- prepare a world for multiplayer or creative work
- avoid common permission problems
- ensure scripting behaves correctly
- prevent accidental damage early on

Think of this as **world initialization**, not software installation.

---

## Step 1: Create the world intentionally

When creating a new world, decide early:
- Creative or Survival
- Singleplayer or Multiplayer
- Experimental vs stable use

These choices affect:
- how permissions behave
- how scripts execute
- how Creative tools are handled

Changing direction later is possible, but planning early saves time.

---

## Step 2: Set default permission levels

Before inviting players:
- decide what a default player can do
- decide who should have elevated access
- avoid giving admin permissions too broadly

A common approach:
- Guests: limited interaction
- Players: normal building
- Admins: setup and maintenance only

Avoid using admin accounts for everyday play.

---

## Step 3: Protect the spawn area

Spawn is the most important area to protect early.

Recommended protections:
- no block breaking
- no block placement
- limited interaction

This prevents:
- accidental damage
- griefing
- broken systems at spawn

Spawn protection should be set **before** players join.

---

## Step 4: Define key areas

Create and document important areas early, such as:
- spawn
- system zones
- Creative build zones
- testing areas

Each area can have:
- custom permissions
- restricted tools
- different interaction rules

Clear area boundaries reduce confusion later.

---

## Step 5: Configure Creative Mode access

If using Creative Mode:
- decide who can use Creative tools
- decide where Creative is allowed
- restrict Creative access in finished areas

Creative Mode is powerful and should be treated like a development tool, not a default playstyle.

---

## Step 6: Verify scripting works

Before writing complex scripts:
- create a simple test script
- trigger it as a non-admin player
- test inside and outside protected areas

This confirms:
- scripts trigger correctly
- permissions are respected
- area restrictions behave as expected

Do not rely on admin-only testing.

---

## Step 7: Test with non-admin accounts

Admins bypass many restrictions.

Always test:
- permissions
- Creative tools
- scripts

using a **normal player account**.

This step catches most setup issues early.

---

## Step 8: Document your setup

If the world is shared or long-term:
- write down permission rules
- list protected areas
- note Creative access rules

Documentation prevents confusion as the world grows.

---

## Common setup mistakes

### Skipping spawn protection
Leads to accidental damage and broken systems.

---

### Giving everyone admin
Hides permission problems and creates security risks.

---

### Testing only in Creative
Scripts that work in Creative may fail in Survival.

---

### Overlapping area permissions
Can cause silent failures and confusing behavior.

---

## When setup is complete

Your world is ready when:
- players can only do what they should
- Creative tools are controlled
- scripts behave consistently
- protected areas work as expected

From here, you can safely:
- build systems
- expand the world
- invite more players

---

## Related pages

- Permissions
- Creative Mode
- Scripting

---

## Need help?

If setup doesn’t behave as expected:
- ask in the Discord: [{{ discord_invite }}]({{ discord_invite }})
- include permission levels and area details
- describe what works and what doesn’t
