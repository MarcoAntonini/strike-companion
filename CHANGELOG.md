# Changelog

## v1.56 — with Strike MOD FW 0.9.1-beta (2026-11-25)
- **New: faster instrument changes (memory fix).** The stock firmware never frees sample memory: every instrument selected, even while browsing, is added, and when the 200 MB fills up the whole kit is wiped and reloaded (up to ~2 minutes from SD). Now only the sounds the kit no longer uses are dropped and the rest are moved together; the kit stays playable and only the new instrument loads. Tested on a 193 MB SD kit.
- LOADING box: the bar now restarts when you switch kits while one is still loading, and it is red until the kit is playable (soft hits available), then turns blue.
- LOADING box fixes: it always closes when the kit has finished loading (an old copy of the box could come back frozen, e.g. "128/195 MB", after the load had finished), and it no longer leaves a faint outline in fading pad glows.
- MOD label now reads "MOD 0.9.1 BETA".
- Strike Companion: Kit Screen Creator Undo / Redo / Reset; trigger-chip update can be unticked; default updater folder Documents\Strike Updater; Tools → Module debug log (for test firmware); the patcher notes when all features are on (the combination tried on a module, minimal testing).

## v1.38 — with Strike MOD FW 0.9.0-beta (2026-11-23)
First public beta. Based on Alesis Strike firmware v1.5.

**Firmware features**
- Hi-hat page: OPEN / CLOSED calibration knobs, RESET (F1), CAL / OUT meters. Calibration is re-sent to the trigger chip at start-up.
- Trigger chip (Patch 7): pedal calibration maths and hi-hat choke fixes.
- Pad trigger pages: CAL / OUT meters with peak hold.
- Custom kit screen from the Kit Screen Creator (up to 23 hit glows). The standard layout matches the stock screen.
- LOADING box: "Preparing kit…", then loaded / total MB, "Initial samples loaded…", "Loading rest of samples…". It stays until the whole kit is loaded.
- Kick Rim (K2H) on the VOICE (Note Chase) and TRIGGER pages.
- "MOD FW 0.9 BETA" label at the top right of the home screen.

**Strike Companion**
- Firmware patcher: the trigger chip update can be unticked (this also unticks the HiHat page knobs, which need it).
- Firmware patcher: the default updater folder path is Documents\Strike Updater.
- Firmware patcher: builds into the updater folder, keeps the originals, and can put the originals back.
- Kit Screen Creator: Undo / Redo (Ctrl+Z / Ctrl+Y), Reset to the standard kit, presets (Standard kit; Example: 7 cymbals), info help, Save for patching. Without a saved layout, the patcher uses the standard layout.
- Kit Editor follows the Kit Screen Creator layout.

**Known limits:** tested on one Strike Pro only; SD card load time unchanged (hardware limited).

## v1.13 – v1.37
- Development builds: firmware research tools, the Kit Screen Creator, the firmware patcher and the hi-hat calibration work that became Strike MOD FW 0.9.0-beta.

## v1.12 — contributed by Marco Antonini (PRs #1 and #2)
- New Practice mode (PRACTICE button, F3): load a Guitar Pro (.gp3 .gp4 .gp5 .gpx .gp) or MIDI drum score and play along. Shows drum notation, a piano roll and a kit picture that lights up as pieces are played.
- Hit scoring with Easy / Normal / Pro strictness, latency calibration, per-bar accuracy heat-map, final report and progress trend.
- Transport with count-in, looping a selected section, "Loop the worst bars", and a metronome (sounds, subdivisions, accents, silent bars; click from the computer, the module or both).
- The score can be played with app sounds, with a kit's sounds, or on the module over MIDI (including the hi-hat pedal). Simulated-player demo and listen-only mode.
- Export a played lesson as .zip (score + results JSON) or as a PDF with notes coloured by result; load a lesson back later.
- Kit picture: piece names can be dragged and resized; "Pedal closed" option to hear closed hi-hat sounds without the module.
- Save As: folder picker listing the SD card's instrument folders; choose where exported kits are saved.
- File menu: save / load app settings (kit layout, names, practice options) to a file; disconnect all drives.
- Fixed some MIDI errors in practice mode.

## v1.11
- Kit Editor: the kit picture sits in a column on the right (drag its edge to resize), pad settings use the space on the left.

## v1.10
- Cleaned up for public release: About box with disclaimer, wording fixes.

## v1.09
- Hi-hat pedal positions follow the factory instruments (decoded from the factory hi-hats); Quick Hi-Hat cymbal and pedal import that sorts samples into positions by file name.

## v1.08
- Undo / redo in both editors, editor buttons in the top bar, compact resizable layout, kit size shown when a kit is selected, hi-hat pedal-position bar with Factory default / Revert.

## v1.07
- All kit settings confirmed (gate time, note off, MIDI channel, FX, EQ/compressor ranges); smaller kit picture; Arrange mode with custom pad names.

## v1.06
- Shows the module's internal drive on the computer via MIDI SysEx (as the Strike Editor does).

## v1.05
- New layout modelled on the Strike Editor: menus, kit picture, knobs, Edit FX, Kit Size, Instrument Editor, Quick Instrument.

## v1.04
- Internal drive and SD card open together; tree view and search; start from a preset and save as a user kit.

## v1.03
- Automatic kit size with 200 MB warning; factory content read-only; new instrument view.

## v1.02 and earlier
- Live hi-hat meter, MIDI-OX log and analysis, trigger settings editor; first kit and instrument editing.
