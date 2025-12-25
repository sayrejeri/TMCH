# Scripting

Scripting allows worlds in **Total Miner Forge** to react dynamically to player actions, events, and game state changes.

Scripts can control:
- logic and automation
- interactive systems
- puzzles and minigames
- custom mechanics
- server-side behavior

Scripting is powerful, but also tightly limited by permissions and context.

---

## What is scripting?

Scripting is the ability to define **custom logic** that runs in response to:
- player actions
- triggers or zones
- world events
- scripted objects or blocks

Scripts do **not** replace game mechanics — they extend them.

---

## Where scripts can run

Scripts typically run in one or more of the following contexts:

- Trigger zones
- Interactive objects
- World-based systems
- Scripted blocks or entities

The exact trigger depends on how the script is set up.

---

## Script execution context

Scripts always run **within a context**.

This context determines:
- who triggered the script
- where it is running
- what permissions apply

Most scripts execute **as the player who triggered them**, not as an admin.

This is one of the most common sources of confusion.

---

## Permissions and scripting

Permissions heavily affect script behavior.

Common rules:
- If a player cannot perform an action normally, a script usually cannot do it on their behalf
- Admins may bypass restrictions that normal players cannot
- Scripts do not automatically elevate permissions

### Example
A script tries to place a block:
- Admin triggers it → works
- Player triggers it → fails

This is usually a **permission issue**, not a script error.

---

## Area restrictions and scripts

Scripts respect **area permissions**.

If a script runs inside a protected area:
- building may be blocked
- interaction may be blocked
- changes may silently fail

Always check area permissions when debugging scripts.

---

## Creative mode and scripting

Creative mode often changes how scripts behave.

In Creative:
- restrictions may be relaxed
- tools may behave differently
- testing is easier

However:
- scripts that work in Creative may fail in Survival
- Creative permissions may hide problems

**Always test scripts in the environment they will be used in.**

---

## Common scripting mistakes

### Testing only as admin
Admins bypass many checks.
This can make broken scripts appear functional.

---

### Ignoring permissions
If a script fails without errors, permissions are often the cause.

---

### Assuming scripts run globally
Scripts usually run locally:
- at a position
- for a player
- within an area

Context matters.

---

### Overcomplicating logic
Simple scripts are easier to debug and maintain.
Complex systems should be broken into smaller parts.

---

## Debugging scripts

When a script doesn’t behave as expected:

1. Test with a non-admin player
2. Check area permissions
3. Verify the trigger is firing
4. Confirm the script context
5. Test outside protected areas

Most issues are configuration-related.

---

## Best practices

### Build small, then expand
Start with simple scripts and layer functionality gradually.

---

### Separate logic from permissions
Design scripts to **assume restrictions**, not bypass them.

---

### Document your scripts
Leave notes explaining:
- what the script does
- where it runs
- what permissions it expects

This helps future maintenance.

---

### Avoid silent failures
If possible, include feedback so players know when an action fails.

---

## When to use scripting

Scripting is ideal for:
- automated systems
- interactive puzzles
- custom mechanics
- event-based logic

It is not ideal for:
- bypassing core game balance
- replacing permission systems
- enforcing rules alone

Use scripting alongside permissions, not instead of them.

---

## Summary

Scripting adds depth and flexibility to Total Miner worlds, but it is constrained by:
- permissions
- area restrictions
- execution context

Understanding those constraints is more important than understanding syntax.

---

## Need help?

If a script isn’t working:
- Ask in the Discord: [{{ discord_invite }}]({{ discord_invite }})
- Share the script context and permissions
- Describe what you expect vs what happens
