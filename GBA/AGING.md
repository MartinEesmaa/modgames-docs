# GBA/AGB Aging Test programs

Written, hacked, analyzed, researched & documented by Martin Eesmaa.

Initial date: 25.10.2026

This test software was used within factory checking process as Nintendo authorized repair centers and to ensure correct operation of all units are tested successfully.

Requirements:

- **AGB Aging Cartridge / TEST PROGRAM Version 1.0, 7.0, 7.1, 9.0 or 10.0 ROM file (mandatory, legal copy)**
- Raster/pixel graphics to edit: GIMP, YY.CHR-NET, Aseprite or any preffered raster graphics editor
- GBA emulator: MesenCE (recommended), please note that almost all emulators of GBA may fail.

## Modding

You are welcome to mod the software aging by replacing text fonts, graphics, edit Mode background via tilemaps and map.

Best to view/emulate/analyze/edit/mod/debug is to use MesenCE emulator.

| Data | Program ROM address | Type | Bytes used |
| --- | --- | --- | ---- |
| Horizontal RGB555 image (240x160) | `$77D70` 1.0 <br> `$83340` 7.0 <br> `$834EC` 7.1 <br> `$84278` 9.0 `$84330` 10.0 <br> | Direct color | 76800 bytes |
| Vertical RGB555 image (160x256) | `$A8F40` 7.0 | Direct color | 81920 bytes |
| Nintendo 64 coin sprite | `$BE180` 7.0 | 8 bps | 4096 bytes |

More coming soon...

- 2026 Martin Eesmaa
