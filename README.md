# NexusShell

> **Terminal-styled YouTube & SoundCloud downloader — paste a link, get the file on your device.**

<img src="https://raw.githubusercontent.com/JTech-CO/Nexusshell/refs/heads/main/images/1-Download.png" width="100%"> 

**▶ Live service: [https://nexusshell.kr](https://nexusshell.kr)**

NexusShell strips away the ads and clutter of typical web downloaders and replaces them with a clean, keyboard-friendly terminal-style interface. Paste a YouTube or SoundCloud link, pick a format, and the file is delivered straight to your device.

> This repository is an **introduction / landing page** for NexusShell. The application's source code (frontend and backend) is **proprietary and not published here** — see [License](#license).

---

## What it does

- **YouTube + SoundCloud** — download from both platforms via a host allow-list.
- **Video or audio** — grab a YouTube video as MP4 or pull the audio; save SoundCloud tracks.
- **Playlists & sets** — queue a whole YouTube playlist or SoundCloud set; files are numbered in order.
- **Live progress** — real-time download progress over WebSocket.
- **Delivered to your device** — the server fetches the media, streams it to your browser, then **auto-deletes its own copy** a short time later. Nothing lingers on the host.
- **No ads, no accounts, no telemetry.**

## How it works

1. Paste a YouTube or SoundCloud URL.
2. NexusShell analyzes it and lists the available formats (or detects a playlist/set).
3. Pick a format and start the download.
4. When it finishes, your browser saves the file to your device automatically (playlists provide a per-file link list).

<img src="https://raw.githubusercontent.com/JTech-CO/Nexusshell/refs/heads/main/images/2-Queue.png" width="100%"> 

## Built with

`Python` · `Flask` · `Socket.IO` · `yt-dlp` · `FFmpeg` · `Docker` · `Caddy`

A lightweight vanilla-JS frontend (no framework) over a Flask + Socket.IO backend, containerized and served behind an auto-HTTPS reverse proxy.

## Use responsibly

NexusShell is intended for personal, fair-use downloads. Using it to reproduce or distribute copyrighted material for commercial purposes may carry legal consequences. Respect the terms of service of the source platforms and the rights of content creators.

## License

**Proprietary — All Rights Reserved.** Copyright © 2026 JTech-CO. See [LICENSE](LICENSE).

The Software may not be copied, reproduced, modified, redistributed, mirrored, hosted, or used to create derivative works, in whole or in part, without prior written permission. This landing page does not grant any right to the application's source code, which is not distributed.

---

<sub>Made by [JTech-CO](https://jtech-co.github.io/) · Live at [nexusshell.kr](https://nexusshell.kr)</sub>
