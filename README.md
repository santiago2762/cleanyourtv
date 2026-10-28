# Anonymous TV theme

A black-and-green Matrix look using the Anonymous artwork supplied by the requester. The wallpaper is darkened to preserve contrast for the clock, app names and dock. The theme uses existing CleanYourTV theme keys and does not require an APK rebuild.

## Install

From the root of the CleanYourTV checkout, with the TV reachable over ADB:

```bash
TV_HOST=192.168.1.50 tools/theme.sh themes/anonymous-tv
```

Replace `192.168.1.50` with the TV's IP address. To remove the theme overlay and return to the built-in configuration:

```bash
TV_HOST=192.168.1.50 tools/theme.sh --reset
```

Windows PowerShell:

```powershell
powershell -ExecutionPolicy Bypass -File tools\theme.ps1 -TvHost 192.168.1.50 themes\anonymous-tv
```

## Design

- Palette: near-black (`#020603`) and Matrix green from the supplied wallpaper.
- Wallpaper: 1920×1080 JPEG, darkened for readability and under the repository's ~300 KB recommendation.
- Layout: five app columns and one row below the dock.
- Motion: normal animation enabled; advanced effects remain off for TV memory/GPU headroom.
- App library enabled.

## Artwork and repository note

`wallpaper.jpg` was prepared from the image provided by the requester for this customization. Rights to redistribute the original artwork have not been independently verified. Before proposing this theme for upstream inclusion, confirm that redistribution is permitted and capture `screenshot.jpg` from a real TV at 1280×720 (not a mock-up), as required by the repository's theme workflow.
