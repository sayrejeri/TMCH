# Permissions

Permissions control **who can do what** in a Total Miner world.  
They affect building, interaction, scripting behavior, server management, and how players interact with each other.

Understanding permissions is essential for:
- multiplayer worlds
- public servers
- creative projects
- preventing griefing or accidental damage

---

## What are permissions?

Permissions are a set of **rules** that determine what actions a player is allowed to perform.

Examples include:
- placing or breaking blocks
- interacting with objects
- using creative tools
- running scripts or commands
- modifying world settings

Permissions are evaluated **every time** a player attempts an action.

---

## Permission levels

Total Miner uses **permission levels** to group abilities together.  
Higher levels generally include the abilities of lower levels.

While exact names and behaviors may vary depending on world configuration, permissions typically follow this structure:

### Guest / Visitor
- Can explore the world
- Limited or no building
- No interaction with protected systems

Used for:
- public exploration
- first-time visitors
- preventing damage

---

### Player
- Can build and interact within allowed areas
- Limited access to tools and systems
- No administrative control

Used for:
- normal survival or creative play
- trusted but non-admin users

---

### Moderator (if configured)
- Can manage players
- Can enforce rules
- May have limited world management abilities

Used for:
- staff members
- community moderation

---

### Admin / Owner
- Full control over the world
- Can modify permissions
- Can access all tools and systems
- Can bypass most restrictions

Used for:
- world owners
- server administrators

---

## Area-based permissions

Permissions can be applied **globally** or **per area**.

This means:
- A player may be allowed to build in one area
- But restricted in another

Area permissions are commonly used for:
- spawn protection
- shops or hubs
- adventure maps
- creative plots

When an action is attempted, Total Miner checks:
1. The player’s permission level
2. The permissions of the area they are in
3. Any overrides or special rules

---

## Permission inheritance and overrides

Permissions often follow a **priority system**.

General rules:
- Area-specific permissions override global permissions
- Higher permission levels override lower ones
- Explicit denies usually override allows

Example:
- A player is allowed to build globally
- But enters a protected area
- The area’s restrictions take priority

Understanding overrides is critical when debugging permission issues.

---

## Common permission-related issues

### “I can build here but not there”
This usually means:
- The area has custom permissions
- The area overrides global settings

Check the area configuration first.

---

### “My script works for admins but not players”
Scripts often respect permission checks.
Possible causes:
- script actions require higher permissions
- script is running in a restricted area
- player lacks interaction permissions

Always test scripts using a non-admin account.

---

### “Players can break things they shouldn’t”
This usually indicates:
- missing area protection
- overly broad permissions
- permissions applied at the wrong level

Use area-based restrictions to limit damage.

---

## Best practices

### Use least privilege
Only give players the permissions they actually need.

---

### Protect important areas
Always protect:
- spawn points
- command areas
- scripted systems
- redstone-like logic setups

---

### Test with non-admin accounts
Admins bypass many restrictions.
Testing only as admin can hide permission issues.

---

### Document your setup
If you run a server:
- document permission rules
- keep a record of custom areas
- make staff aware of overrides

This prevents confusion later.

---

## Permissions and creative mode

Creative mode tools are often restricted by permissions.
This prevents:
- accidental world damage
- abuse of powerful tools
- unintended script activation

If creative tools don’t work:
- check the player’s permission level
- check area restrictions
- confirm creative access is enabled

---

## Permissions and scripting

Scripts may:
- check player permissions
- fail silently if permissions are insufficient
- behave differently for admins vs players

Always assume scripts run under **the permissions of the player triggering them**, unless explicitly designed otherwise.

---

## Troubleshooting checklist

If something doesn’t work:
1. Check the player’s permission level
2. Check the area permissions
3. Look for overrides
4. Test outside protected areas
5. Test with a non-admin account

Most permission issues are caused by **overlapping rules**, not bugs.

---

## Summary

Permissions are the backbone of world control in Total Miner.

They determine:
- who can build
- who can interact
- who can manage systems
- how scripts behave

A clear permission structure makes worlds safer, cleaner, and easier to manage.

---

## Need help?

If you’re unsure how permissions are behaving:
- Ask in the Discord: [{{ discord_invite }}]({{ discord_invite }})
- Check related system pages
- Share details about your setup so others can help
