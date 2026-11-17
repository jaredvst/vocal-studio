# Vocal Studio 0.1.0 — Installation

Vocal Studio is a complete vocal chain in one plugin. Each download contains the plugin, a standalone app, the user manual and the licence.
Everything the plugin needs, including its interface, is inside the plugin file. There are no extra asset folders to copy.

## Windows (10 / 11, 64-bit)

**Plugin (VST3):** copy the whole `Vocal Studio.vst3` folder to

    C:\Program Files\Common Files\VST3\

Windows asks for administrator permission to copy into this folder. Then rescan plugins in your DAW. In FL Studio: *Options → Manage plugins → Find installed plugins*.

**Standalone app:** `Vocal Studio.exe` runs from anywhere. Choose your audio interface under *Options → Audio/MIDI settings*.

**Requirement:** the Microsoft Edge WebView2 Runtime. It's built into Windows 11 and installed on almost every up-to-date Windows 10 PC. If the plugin window stays blank, install the free "Evergreen" runtime from Microsoft's WebView2 page.

## macOS (11 Big Sur or later, Apple Silicon and Intel)

Copy:

| File | To |
|---|---|
| `Vocal Studio.vst3` | `/Library/Audio/Plug-Ins/VST3/` |
| `Vocal Studio.component` (Audio Unit: Logic, GarageBand) | `/Library/Audio/Plug-Ins/Components/` |
| `Vocal Studio.app` | `/Applications/` |

This release isn't notarised by Apple. If macOS says the plugin "can't be opened" or "is damaged", run this once in Terminal, then rescan in your DAW:

    sudo xattr -dr com.apple.quarantine "/Library/Audio/Plug-Ins/VST3/Vocal Studio.vst3" "/Library/Audio/Plug-Ins/Components/Vocal Studio.component" "/Applications/Vocal Studio.app"

## Linux (64-bit)

Copy `Vocal Studio.vst3` to `~/.vst3/` (only you) or `/usr/lib/vst3/` (all users). The standalone `Vocal Studio` binary runs from anywhere: `chmod +x "Vocal Studio"` if needed.
It needs WebKitGTK for its interface (`libwebkit2gtk-4.1-0`, which is installed with most desktops).

## Your presets

Presets you save are stored in your Documents folder under `Vocal Studio/Presets/<section>/`. Back up that folder to keep them.

## Upgrading from VocalForge (pre-release testers)

Vocal Studio is the same plugin with a new name. DAW projects that used VocalForge open it automatically, and your saved presets are copied over the first time it runs.
Remove the old `VocalForge*.vst3` files from your VST3 folder so your DAW doesn't list the plugin twice.

## Uninstall

Delete the files you copied above. Your presets in Documents stay until you delete that folder.
