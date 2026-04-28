# Patch34: Brickwall Limiter

*Impossible Geometry Series: ESCHER*

<p align="center">
  <img src="assets/ui.png" alt="Patch34 Brickwall Limiter UI" width="620">
</p>


Scripts and tools for REAPER. Useful, weird, and everything in between.

---

Sample-peak brickwall limiter with a custom Escher-inspired JSFX interface. Part of the Impossible Geometry Series.

## Features

- Sample-peak brickwall limiting
- Input gain control
- Output ceiling control
- Release time control
- Custom Escher-inspired vertical UI
- Built-in input/output peak display
- Gain reduction display
- Scalable JSFX graphics window
- No ReaImGui required
- No js_ReaScriptAPI required
- macOS & Windows compatible

### Input

Adjusts signal level before limiting.

Range: `-24 dB` to `+24 dB`

### Output Ceiling

Sets the limiter ceiling.

Range: `-24 dBFS` to `0 dBFS`

### Release

Controls limiter release time.

Range: `1 ms` to `500 ms`

---

## Metering

The interface includes:

- **Input Peak** — pre-limiter peak level
- **Output Peak** — post-limiter peak level
- **Gain Reduction** — amount of limiting applied

REAPER’s external JSFX host meters are intentionally hidden so the plugin can use its own custom visual layout.

---

## Demo

A short demo video is included here:

[Open demo video](assets/patch34-brickwall-limiter-demo.mov)

---

## Installation

Copy `Patch34_Brickwall_Limiter.jsfx` to your REAPER Effects folder:

macOS  
`~/Library/Application Support/REAPER/Effects/`

Windows  
`%APPDATA%\REAPER\Effects\`

Linux  
`~/.config/REAPER/Effects/`

Then rescan JSFX in REAPER:

**Options → Preferences → Plug-ins → ReaScript / JS → Re-scan**

The plugin will appear as:

`JS: Brickwall Limiter`

---

## Workflow

1. Insert **JS: Brickwall Limiter** on a track.
2. Set **Input** to drive the limiter.
3. Set **Output Ceiling** to the desired maximum level.
4. Adjust **Release** until gain reduction feels natural for the source.
5. Watch the built-in peak and gain-reduction meters.

---

## Files

- `Patch34_Brickwall_Limiter.jsfx` — REAPER JSFX plugin
- `assets/ui.png` — README preview image
- `assets/patch34-brickwall-limiter-demo.mov` — short demo video

---

## License

MIT
