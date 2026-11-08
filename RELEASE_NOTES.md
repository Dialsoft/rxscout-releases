# RX Scout release notes

## 1.1.0 - November 7, 2026

- **Interface colors**: pick from nine color schemes (Royal Purple, Ocean Blue, Teal, Forest Green, Crimson, Sunset Orange, Retro Amber, Hot Pink, Graphite) or any custom color, under Settings > Colors. The header, buttons, highlights and tabs change instantly, and every color has matching shades for both Light and Dark themes.
- On Android the phone's status bar matches the chosen color.

## 1.0.0 - November 7, 2026

First release. Windows (single portable EXE) and Android.

### Control
- **Main Zone** page: power, big volume readout and slider, mute, sleep timer, input tiles (shows your renamed input names), SCENE buttons, Cinema DSP program picker with a plain-English description of each program, Straight / Enhancer / Pure Direct / Adaptive DRC toggles, and Now Playing with album art for network sources.
- **Zone 2** page: power, volume, mute, input and sleep for the second zone.
- **Sources** page: FM/AM tuner (type a frequency, seek, presets), and menu browsing for Net Radio, Server (DLNA), USB, iPod, Pandora (thumbs up/down), SiriusXM and Rhapsody, with repeat/shuffle where supported.
- **Sound** page: bass, treble, subwoofer trim, Adaptive DRC, CINEMA DSP 3D, Extra Bass, YPAO Volume, Dialogue Lift and Dialogue Level.

### Undocumented features (found on the RX-V677, firmware 1.98/1.4)
- **Speaker channel levels and distances** - normally only reachable in the on-screen setup menu.
- **Per-input volume trim** for every input.
- **Front display dimmer** and short-message on/off.
- **Maximum volume** and **power-on volume** for each zone.
- **HDMI Control (CEC)**, **HDMI standby pass-through** and **HDMI output resolution**.
- **ECO mode**.
- **Network details** including the MAC address (for DHCP reservations).
- **Firmware version** read directly from the receiver.
- Every undocumented write is read back afterwards so you know whether the receiver kept the value.

### Tools
- **Command Explorer**: the receiver's full published command list as a searchable tree; click to load any command, then send it. Raw XML console with GET/PUT, formatting and copy.
- **Discover hidden commands**: read-only scanner that tries every published path plus ~70 extra names used by other Yamaha models and reports which ones answer.
- **Remote-code injection** (experimental): make the receiver act on an IR remote code.
- **Back up / restore settings**: save tone, DSP, trims, speaker levels, display, HDMI, names and volume limits to a file; restore shows a side-by-side diff and writes only what you tick.
- **Export snapshot**: every readable answer in one JSON file.
- **Traffic log**: every command and the receiver's exact answer, with return-code explanations.

### App
- Ribbon (Home, Sound, Tools, Settings, Help) plus page tabs; ribbon can be collapsed.
- Finds receivers automatically (UPnP/SSDP, then a subnet sweep), or add one by IP. Remembers several receivers.
- Verbose tooltips on every control (long-press on Android); can be switched to short or off.
- All settings apply live: refresh speed, volume step, **volume safety limit**, light/dark theme, start page.
- Keyboard: Up/Down or +/- for volume, M for mute, F5 to refresh (Windows).
- Phone volume keys control the receiver while RX Scout is open (Android, can be turned off).
- Auto-update check with SHA-256 verification (Windows installs itself; Android opens the download).
