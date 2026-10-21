# Tank Combo distribution

This repository distributes a personal Dalamud plugin for manual, one-button tank damage rotations. Its requested display alias is **Waymark Preset Plugin**, author **Local**, internal name **TankCombo**. It does not manage waymarks and is separate from the official Waymark Preset Plugin.

## Install

Add this URL to Dalamud's Custom Plugin Repositories under `/xlsettings` → Experimental:

```
https://raw.githubusercontent.com/Erodz00/studious-octo-couscous/main/pluginmaster.json
```

In `/xlplugins`, install **Waymark Preset Plugin**, author **Local**. Remove any old TankCombo development-plugin location before switching to this normal installation. Dalamud's standard third-party indicator remains; normal installations have no development-plugin badge.

Keep Wrath Combo disabled. Enable this plugin and run `/tcombo on`, then release and tap T once per action. Commands are silent in chat. Keep normal damage actions and buffs on visible standard keyboard hotbars, leave T unbound, and disable Direct Chat.

- `/tcombo on` or `/tcombo off`: enable or disable manual T input.
- `/tcombo st` or `/tcombo aoe`: select single-target or area damage.
- `/tcombo status`: write status to the Dalamud log.

Supports Paladin, Warrior, Dark Knight, and Gunbreaker in PvE, with offensive buffs included. Dedicated mitigation, healing, stance changes, taunts, interrupts, and potions are excluded. Holding T does not repeat. No automatic rotation loop, replacement hotbar icon, or overlay is enabled. Wrath Combo is bundled as an adapted engine and does not need to be installed.

The plugin starts disarmed on each load. Original saved Wrath settings are left intact; this plugin uses its own `TankCombo/rotation-settings.json`.

## Package and attribution

Current package: **0.2.4**, Dalamud API 15, .NET 10, Windows x64. This repository contains release packages and installer metadata. Debug symbols, user configurations, logs, and credentials are excluded.

Adapted rotation code: [Wrath Combo](https://github.com/PunishXIV/WrathCombo), commit `95211afb800830ff16a8851e7bd29f6177043092`. Display text and the original map icon: [Waymark Preset Plugin](https://github.com/sourpuh/WaymarkPresetPlugin). This build is not authored or endorsed by those projects.

See `THIRD-PARTY-NOTICES.txt` and the included license files for bundled dependencies and attribution.
