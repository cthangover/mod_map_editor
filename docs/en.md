# World Map Editor — zones, markers and labels of the world map

The World Map Editor draws the travel map of `map_base` over the running game: region polygons, markers and labels, each with a title, a description, the scene it leads to and whether it is locked or hidden. A preview shows the map exactly as the player will see it, and **Refresh in-game map** puts saved changes into the running game.

This tool is for the world map. Tile maps of the RPG world are edited by the RPG map editor (`rpg_editor`).

## Opening it

Hammer button on the in-game toolbar → **Map Editor**.

## Editing the map

![The World Map Editor on the cthangover map: the zones home, home_label, town_entry and town_entry_label on the left, the region of the villa selected on the map with its vertices, and its properties on the right: scene home_outside, availability, In game: open.](assets/map-editor.jpg)

1. Pick a mod and a map file (`map/*.json`) in the selector.
2. **+ Region** (or **Draw**) and click the map to place vertices; double-click, Enter or Esc finishes, RMB removes the last vertex. **+ Marker** and **+ Label** add the other zone kinds.
3. Select a zone in **Zones** or on the map. In **Zone properties** set its ID, **Title** and **Description** (locale keys; a missing translation is flagged), its **Scene**, and **Availability**: *Locked for travel* or *Hidden from the map*. The **In game:** line tells what the player will actually get (open, locked by the flag, locked because the scene is missing, hidden).
4. Drag zones and vertices on the map; RMB on a vertex deletes it, Del deletes the zone.
5. **▶ As in game** shows the map as the player sees it — hover, zone card, markers — including unsaved edits.
6. Ctrl+S saves; **Refresh in-game map** re-reads the saved files in the running game.

## Limits

- Folder mods only; packed mods are read-only.
- Titles and descriptions are locale keys; their texts are edited in the mod's locale files.

## Dependencies

`tools_base`, `map_base`, `ui_base`.
The older `editor_tools` package installs this mod together with the other authoring windows.
