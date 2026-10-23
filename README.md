English | [简体中文](README.zh-CN.md)

# codex-claude-muse-boot

**Boot / startup splash animations for AI coding tools — Codex, Claude and Muse character-splash editions, in one dependency-free HTML file.**

[![Stars](https://img.shields.io/github/stars/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/stargazers)
[![Forks](https://img.shields.io/github/forks/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/network/members)
[![Last commit](https://img.shields.io/github/last-commit/chenyi6758-source/codex-claude-muse-boot?style=flat)](https://github.com/chenyi6758-source/codex-claude-muse-boot/commits/main)
[![License](https://img.shields.io/github/license/chenyi6758-source/codex-claude-muse-boot?style=flat)](LICENSE)
[![Live demo](https://img.shields.io/badge/Live%20demo-demo.cyruscy.me-brightgreen)](https://demo.cyruscy.me/)

A set of "OS boot ceremony" splash animations for AI tools — as **character splashes**: an illustrated character fades in, a script signature and a one-line motto appear, the hand-drawn mark traces itself into shape, metallic title letters land, a terminal boot log scrolls, and the chat box rises into the final frame. Three editions, one file, everything generated in code.

All marks are hand-drawn, same-style graphics; no official assets are used.

## Demo

**▶ Live demo: https://demo.cyruscy.me/**

Or open `index.html` in any modern browser. No build step, no dependencies, no server needed. The three stages autoplay side by side and can be replayed, paused and speed-shifted (0.5× / 1× / 2×) individually or in sync. Each stage runs ≈ 6.8 s; the whole page is one ~86 KB HTML file plus three character artworks (1920 × 1280).

| Muse — "Cyrus" | Codex | Claude |
|---|---|---|
| ![Muse character](assets/char-muse.webp) | ![Codex character](assets/char-gpt.webp) | ![Claude character](assets/char-claude.webp) |

The original logo-only version is preserved at [`index-v1-original.html`](index-v1-original.html) (live: https://demo.cyruscy.me/index-v1-original.html).

## Features

- **Three character-splash stages** — Muse (spark mark, royal blue, resident character *Cyrus*), Codex (hex-knot mark, classic green, "Build Mode"), Claude (terracotta-orange starburst, "Deep Thinking Mode"), each with its own capability rail, terminal boot log and motto line
- **Matrix rain mode** — a global toggle that turns every screen into cascading katakana/digit rain while the boot log types itself out
- **Stage effects** — glitch, particle stardust convergence, neon grid, light-track scan, dissolve outro, and more
- **Material workbench**
  - 11 procedurally generated themes (deep-sea aurora, neon rainy night, matrix code rain, …) — zero stock assets needed
  - Live image search via **Wikimedia Commons** (default) and **Openverse** (backup) — both free, no API key; click a result to use it as the boot background
  - **Upload & animate**: drop your own image or video, pick one of 10 motion presets and a duration — your media becomes the boot animation, processed locally in memory, never uploaded anywhere
  - **Steam Wallpaper Engine import**: paste a Workshop link to parse its item ID, get the local path (`steamapps/workshop/content/431960/<ID>`) and a `steam://` deep link, then drop the downloaded wallpaper file into the upload zone

## On Windows & macOS

This page itself is platform-neutral — any modern browser, either OS, nothing to install. If you want a splash in front of the real desktop apps, the practical routes differ by platform:

- **Windows** — deep integration is possible: launcher-style tools can sit in front of the app (fullscreen intro, then hand off), boot-animation plugins that accept a custom video clip can play a stage recorded/exported from this page, and Wallpaper Engine wallpapers can be turned into a boot background with the built-in import above.
- **macOS** — the overlay route: a launcher plays the intro in its own window and hands off with a fade, without modifying the app itself. Unsigned local apps need a first-launch right-click → Open (Gatekeeper). The web demo above is the zero-install route on Mac.

## Why

Boot animations for AI tools are a scattered niche: a cluster of plugins exists for one harness, a launcher or two for Codex, almost nothing for Claude, and nothing at all for Muse. This repo collects the concept for all three in one place and keeps it hackable: one file, readable code, everything generated in code.

## Roadmap

- [ ] Demo GIFs of the three stages at the top of this README
- [ ] Export a composed stage as MP4 / WebM / GIF (usable as a DSH plugin clip)
- [ ] Downloadable asset pack: character PNGs + stage recordings
- [ ] Time-of-day intro variants and a clip-library / rotation mode
- [ ] Standalone launchers for the Codex / Claude desktop apps on Windows (fullscreen intro, then hand off to the app)
- [ ] More brand stages and community themes

## License

MIT for the code. The character artworks in `assets/` were AI-generated for this project. Media fetched through Wikimedia Commons / Openverse keeps its own per-item license — check the license shown with each result before reusing it elsewhere.
