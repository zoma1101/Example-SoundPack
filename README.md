## Example SoundPack for Music Player Mod

This **Example-SoundPack** is intended to be placed in the `soundpacks` folder when using the [Music Player Mod](https://example.com).

> ⚠️ Due to copyright restrictions, the included `.ogg` files are *non-playable placeholders*.  
> When creating your own soundpack, please replace them with valid `.ogg` files that can be legally used and played in-game.

---

### Basic Structure

Each soundpack contains:

- A `music` folder: Place your `.ogg` files here.
- A `conditions` folder: Place your `.json` condition files here to define when each track should be played.

---

### Supported Conditions
| Key           | Type                     | Description |
|----------------|--------------------------|-------------|
| `biomes`       | `string[]`               | The track will play in the specified biomes. Biome tags are supported. |
| `is_night`     | `true` / `false`         | Plays only at night if `true`. |
| `is_combat`    | `true` / `false`         | Plays during combat if `true` (e.g., nearby hostile mobs preparing to attack). |
| `isVillage`    | `true` / `false`         | Plays when villagers are nearby if `true`. |
| `min_y`        | `number`                 | Plays when player is above the specified Y-level. |
| `max_y`        | `number`                 | Plays when player is below the specified Y-level. |
| `weather`      | `["clear", "rain", "thunder"]` | Plays during the specified weather condition(s). |
| `dimensions`   | `string[]`               | Plays in the specified dimensions. |
| `gui_screen`   | `string[]`               | Plays only while the specified GUI screen is open. Valid values: `crafting`, `brewing_stand`, `shulker_box`, `furnace`, `anvil`, `enchantment`, `cartographytable`, `smithing`, `merchant`. |
