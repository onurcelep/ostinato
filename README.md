# 𝄆 etude 𝄇

**A private, offline practice looper for musicians.** Open a local video or audio file, loop a passage, slow it down, and change the key — all in your browser. Nothing is uploaded; your files never leave your device.

> *étude* — a piece written to practice a skill. That's the whole idea.

**▶ Live:** https://onurcelep.github.io/etude/

## Features

- **Loop sections (A–B)** — mark a start and end, loop it instantly; save named loops and switch between them.
- **Transpose & pitch** — shift by semitones (and fine cents) without changing speed, powered by [SoundTouchJS](https://github.com/cutterbl/SoundTouchJS).
- **Speed** — 25%–200% with "keep pitch" (time-stretch), and an optional song-BPM readout.
- **On-video controls** — set A/B and toggle the loop right from the player.
- **History** — recent files are remembered locally (stored in your browser via IndexedDB) and reopen instantly.
- **Installable PWA** — add it to your home screen / dock and it runs offline in its own window.
- **Responsive** — works on desktop and mobile.
- **100% client-side** — no server, no accounts, no tracking.

## Use it

Open **https://onurcelep.github.io/etude/** (or open `index.html` directly).
Drop a file (or click to browse), set your loop, and practice.

**Install (optional):** on desktop, use your browser's *Install* option; on mobile, *Share → Add to Home Screen*. It then works fully offline.

> Note: the transpose/pitch engine uses an AudioWorklet when served over `http(s)` and falls back to a ScriptProcessor when opened directly from `file://`, so it works either way.

## Tech

A static site with no build step and no dependencies to install: a self-contained **`index.html`** (HTML/CSS/JS with the pitch/tempo engine, [SoundTouchJS](https://github.com/cutterbl/SoundTouchJS), bundled inline) plus PWA assets (`manifest.json`, `sw.js`, icons).

## License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE).
It bundles **SoundTouchJS**, which is licensed under **LGPL-2.1**; its notice is preserved inline and it remains under its own license.

## Support

If etude helps your practice, you can [buy me a coffee ☕](https://buymeacoffee.com/onurcelep).
