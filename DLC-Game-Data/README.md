# DLC-Game-Data

Source data for the BattleTech DLC content shown in BattleTech Field Manual:
Flashpoint, Urban Warfare and Heavy Metal.

## Provenance

- Copied from `github.com/caardappel-hbs/bt-dlc-designdata`, commit `fbce5df`
  (25-Feb-2020), published by a Harebrained Schemes developer under the MIT
  licence. The licence is kept here as `LICENSE-bt-dlc-designdata`.
- Only the folders the app uses were copied: chassis, mech, weapon, upgrades,
  jumpjets, ammunition, ammunitionBox, hardpoints, movement. Contracts,
  flashpoints, events, vehicles and milestone data were left out.
- Files are unmodified. Some contain trailing commas and will not parse with a
  strict JSON parser until those are stripped.

## Known limitations

This is 2019 authoring-time data, not the data that shipped in the game. Known
differences:

- Chassis files report 0 heat sinks. The app assumes the standard base
  dissipation for DLC mechs.
- `Weapon_Mortar_Thumper.json` is incomplete (its display name reads "AC/10").
- Values that differ from the shipped game cannot be detected from this source
  alone.

Base-game data lives in `../game-source/`.
