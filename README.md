English | [简体中文](README.zh-CN.md)

# AI Boot Animations

**Cinematic boot / startup animations for AI assistants — Muse, ChatGPT and Claude editions, in one dependency-free HTML file.**

Inspired by the viral DeepSeek Harness boot-animation plugins, this project recreates that 6-second "OS boot" ceremony for the AI assistants that *don't* have an open plugin system: a light sweep, a hand-drawn mark tracing itself into shape, metallic title letters, a terminal-style loading log, a progress bar, and a chat box rising into the final frame.

> **Unofficial fan-made concept.** Not affiliated with Meta, OpenAI or Anthropic. All marks are hand-drawn, same-style graphics; no official assets are used. Muse, ChatGPT and Claude have no open boot-animation plugin API — this is a playable concept demo and a starting point for launcher/desktop integrations.

## Demo

**▶ Live demo: https://chenyi6758-source.github.io/ai-boot-animations/**

Or open `index.html` in any modern browser. No build step, no dependencies, no server needed. The three stages autoplay side by side and can be replayed, paused and speed-shifted (0.5× / 1× / 2×) individually or in sync.

## Features

- **Three brand stages** — Muse (spark mark, royal blue, "Inspiration Work Mode"), ChatGPT (hex-knot mark, classic green, "Professional Work Mode"), Claude (terracotta orange starburst, "Deep Thinking Mode"), each with its own capability rail and terminal boot log
- **Matrix rain mode** — a global toggle (plus a stage-effect option and a theme preset) that turns every screen into cascading katakana/digit rain while the boot log types itself out character by character
- **Stage effects** — glitch, particle stardust convergence, neon grid, light-track scan, dissolve outro, and more
- **Material workbench**
  - 11 procedurally generated themes (deep-sea aurora, neon rainy night, matrix code rain, …) — zero stock assets needed
  - Live image search via **Wikimedia Commons** (default) and **Openverse** (backup) — both free, no API key; click a result to use it as the boot background
  - Directory of more free material sites (Pexels, Pixabay, Coverr, Mixkit, Videvo) with honest notes on which need your own API key
  - **Upload & animate**: drop your own image or video, pick one of 10 motion presets (slow push-in, pan, breathing, glitch, stardust, neon, light scan, dissolve, VHS, still) and a duration — your media becomes the boot animation, processed locally in memory, never uploaded anywhere
  - **Steam Wallpaper Engine import**: paste a Workshop link to parse its item ID, get the local path (`steamapps/workshop/content/431960/<ID>`) and a `steam://` deep link, then drop the downloaded wallpaper file into the upload zone. (Wallpaper Engine offers no web API to read a Workshop library directly — local import is the real, working route.)

## Why

On GitHub, boot-animation plugins exploded only where a platform made them installable: DeepSeek Harness has 20+ such repos (the original at 300+ stars within a month), while ChatGPT/Codex has a handful of 0–1 star attempts, Claude has three tiny projects, and Muse has none. This repo collects the concept in one place and keeps it hackable: one file, readable code, everything generated in code.

## Roadmap

- [ ] Standalone launchers for the ChatGPT / Claude desktop apps on Windows (fullscreen intro, then hand off to the app)
- [ ] Auto-scan of the local Wallpaper Engine Workshop folder in a desktop build
- [ ] Export the composed animation as a video / GIF
- [ ] More brand stages and community themes

## License

MIT for the code. Media fetched through Wikimedia Commons / Openverse keeps its own per-item license — check the license shown with each result before reusing it elsewhere.
