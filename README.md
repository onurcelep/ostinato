# 𝄆 ostinato 𝄇

**A private, offline practice looper for musicians.** Open a local video or audio file, loop a passage, slow it down, and change the key — all in your browser. Nothing is uploaded; your files never leave your device.

> *ostinato* — a musical pattern that repeats persistently. That's the whole idea.

## Features

- **Loop sections (A–B)** — mark a start and end, loop it instantly; save named loops and switch between them.
- **Transpose & pitch** — shift by semitones (and fine cents) without changing speed, powered by [SoundTouchJS](https://github.com/cutterbl/SoundTouchJS).
- **Speed** — 25%–200% with "keep pitch" (time-stretch), and an optional song-BPM readout.
- **On-video controls** — set A/B and toggle the loop right from the player.
- **History** — recent files are remembered locally (stored in your browser via IndexedDB) and reopen instantly.
- **100% client-side** — no server, no accounts, no tracking. Works offline.

## Use it

Just open **`index.html`** in any modern browser, or visit the hosted version.
Drop a file (or click to browse), set your loop, and practice.

> Note: the transpose/pitch engine uses an AudioWorklet when served over `http(s)` and falls back to a ScriptProcessor when opened directly from `file://`, so it works either way.

## Tech

A single self-contained `index.html` — plain HTML/CSS/JS, no build step, no dependencies to install. The pitch/tempo engine ([SoundTouchJS](https://github.com/cutterbl/SoundTouchJS)) is bundled inline.

## License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE).
It bundles **SoundTouchJS**, which is licensed under **LGPL-2.1**; its notice is preserved inline and it remains under its own license.

## Support

If ostinato helps your practice, you can [buy me a coffee ☕](https://buymeacoffee.com/onurcelep).
