# Custom Distance for Start - Updated

An update of Jerzat's Custom Distance for Start mod, adding three Advanced Setup options that set the minimum starting distance between civilizations and city-states.

## Availability

- [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3427012096)
- [Nexus Mods](https://www.nexusmods.com/civilisationvi/mods/303)

## What It Does

- Adds three options to the Advanced Setup screen's map settings: minimum starting distance between players, minimum distance between city-states, and minimum distance between players and city-states.
- Enforces those distances at map generation by fully overriding the base game's `AssignStartingPlots.lua`.
- Its hardcoded placement checks use your values instead, for player-to-player, city-state-to-player and city-state-to-city-state placement.
- On water maps the player-to-city-state minimum is applied one tile lower than the value you set.
- The values apply only when a map is generated, so enabling the mod changes nothing in a game already started.

## Requirements

Civilization VI with the Standard, Rise and Fall or Gathering Storm ruleset. The option labels and descriptions are in English only.

## Installation

- **Manual:** copy the `Custom Distance for Start - Updated` folder into `%USERPROFILE%\Documents\My Games\Sid Meier's Civilization VI\Mods\`, then enable it under Additional Content.

## Configuration

The three options appear on the Advanced Setup screen once the mod is enabled:

- Min. starting distance between players (default 9). Values above 15 may fail to place some players at that distance on smaller or less land-rich maps.
- Min. distance between city-states (default 5). Values above 10 may leave some city-states unable to spawn.
- Min. distance between players and city-states (default 7). Values above 10 carry the same risk.

## Compatibility

- Fully overrides `AssignStartingPlots.lua`, so it conflicts with any other mod or map generator that also overrides that file.
- Incompatible with Yet (not) Another Maps Pack (YnAMP): it replaces the same file and takes priority, so the distance options do nothing while it is enabled.
- Tested beside Sukritact's Oceans, Terra Mirabilis and BD - Wetlands on Gathering Storm: the distance options work with each.
- Does not affect saved games, so it can be enabled or disabled between games without breaking existing saves.

## License

License terms are in the [Alkeari License Agreement](https://gist.github.com/Alkeari/2c6ec0cdf3dafee375b1a00b28ca190a).
