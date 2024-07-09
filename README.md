# Zombat

# Zombat Combat System 🛡️

Enhance your Minecraft PvP experience with the Zombat Combat System! This powerful plugin ensures fair and balanced combat by enforcing specific rules and limitations during player battles. Perfect for survival and PvP servers, Zombat Combat System adds a new layer of excitement and challenge to your Minecraft world.

## Features 🌟

- **Combat Mode Activation:** Automatically puts players in combat mode for 20 seconds after they engage in battle, preventing them from using certain commands and items.
  
- **Action-Bar Timer:** Displays a customizable timer in the action bar, showing players how long they remain in combat.
  
- **Command Restrictions:** Blocks the use of specific commands (e.g., tp, tpa, spawn) during combat to prevent unfair advantages.
  
- **Custom Messages and Sounds:** Provides configurable messages and sounds for various combat events, such as leaving combat or attempting to use blocked commands.
  
- **Ender Pearl Usage Control:** Option to disable Ender Pearl usage during combat, ensuring players cannot escape unfairly.
  
- **Permission-Based Bypasses:** Allows players with specific permissions (`zombat.admin`, `zombat.bypass`) to bypass combat mode restrictions, ideal for server staff and trusted players.
  
- **Ignored Worlds:** Specify worlds where the combat system should be disabled, allowing for designated safe zones or specific gameplay areas.

## Configuration Example 📝

```yaml
Combat:
  Enabled: true
  Duration: 20 # The Duration how long a Player should be in Combat.

  Action-Bar: "&7Combat #0078FF%timer%" # The Message that will be Displayed in the Actionbar.
  Blocked-Commands: # Commands that are not allowed to use in Combat.
    - tp
    - tpa
    - spawn
    - rtp
    - shop
    - gamemode
    - gmc
    - gms
    - gmsp
    - gma

  Messages:
    Left-Combat: "&7You Left Combat"
    Blocked-Message: "#FF0000You can't use that Command in Combat!"
    Ender-Pearls: "#FF0000You can't use Ender Pearls in Combat!"
  Sounds:
    Left-Combat: "ENTITY_VILLAGER_NO"
    Blocked-Message: "ENTITY_VILLAGER_NO"
    Ender-Pearls: "ENTITY_VILLAGER_NO"
  Utils:
    Ender-Pearls: true # Should Players use Ender Pearls in Combat? true for yes and false for no
    Ignore-Ops: false
    BypassAdmin: false # Should Players with the Permission zombat.admin be set in Combat if they get attacked?
    Bypass: true # Should Players with the Permission zombat.bypass be set in Combat if they get attacked?

  Ignored-Worlds:
    - "spawn"
    - "pvp"
```

Ensure fair play and enhance your PvP encounters with the Zombat Combat System, your ultimate combat control solution for Minecraft servers! ⚔️
