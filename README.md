# Strike Companion

A free, unofficial editor for the **Alesis Strike / Strike Pro** drum module that runs in your web browser.
It is laid out like the Alesis Strike Editor and adds live MIDI tools.

> **Not affiliated with, endorsed by or supported by Alesis or inMusic.** Alesis and Strike are trademarks of their owners.
> File formats were worked out independently, for compatibility. Use at your own risk and keep backups.

## What it does

- **Kit Editor**: browse preset (internal) and user (SD card) kits, edit every pad: layers A/B, level, pan, decay, pitch, filter, velocity, FX sends, playback, MIDI out. Edit the kit's Reverb, FX1, FX2 and EQ/Compressor.
  Shows the kit's sample-memory size and warns when it goes over the module's 200 MB limit. Clickable kit picture you can arrange to match your own kit.
- **Instrument Editor**: hi-hat pedal positions (Open / Semi-open / Closed) on one draggable bar, velocity ranges, round robin / random, import WAV samples (converted to 48 kHz / 16-bit), Auto-Map by loudness, Quick Instrument.
- **Live tools**: hi-hat pedal meter (CC 4) with zones, pad hit meters, MIDI log saved in MIDI-OX format, log analysis, and the trigger-settings dump (SysEx 0x0D): receive, edit, save as .syx, send.
- Undo / redo, a list of every change before you save, and backups of files it overwrites.

Preset (internal) content is never written. New and edited kits and instruments are saved to the module's SD card.

## How to use

1. Download `index.html` (or use the GitHub Pages link, if enabled) and open it in **Chrome or Edge** on a computer. Firefox and Safari don't support Web MIDI / folder access.
2. Connect the Strike by USB and switch it on.
3. Click **Connect MIDI** and allow MIDI with SysEx. The page then asks the module to show its internal drive on the computer.
4. **File → Connect Strike drives…** and select the module's drives (internal and SD card). The page remembers them.

No module handy? **File → Open Factory Content Update (.bin)** loads the preset kits and instruments from an official Alesis content-update file, read-only.

## Status

Tested against copies of a Strike Pro SD card and the v1.3 factory content update. Features marked as experimental:

- Showing the internal drive over MIDI (uses the same SysEx message as the Strike Editor; not yet confirmed on every setup).
- Curve names marked “?” in Trigger settings are inferred, not confirmed.

Please report results and problems in **Issues**.

## Privacy

Everything runs locally in your browser. Nothing is uploaded. Settings (layout, remembered drives) are kept in your browser's local storage.

## Not included

This repository contains no Alesis firmware, software, samples or content. You need your own module and its files.

## Licence

See [LICENSE](LICENSE).
