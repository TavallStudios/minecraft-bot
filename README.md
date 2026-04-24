# minecraft-bot

<!-- tavall:badges:start -->
[![Org](https://img.shields.io/badge/org-TavallStudios-181717?logo=github)](https://github.com/TavallStudios) [![Stack](https://img.shields.io/badge/stack-Node-0A7BBB)](https://api.github.com/repos/TavallStudios/minecraft-bot) ![History](https://img.shields.io/badge/history-preserved-6f42c1)
<!-- tavall:badges:end -->

Node.js bot harnesses for exercising Minecraft server connection flows and game-mode smoke tests. The repository is split into focused scripts for CTF scenarios, Java Edition smoke checks, Bedrock smoke checks, and shared harness code.

## What It Does

- Starts scripted Minecraft bot flows against local or remote test servers.
- Groups CTF-specific automation separately from general Java and Bedrock connection smoke tests.
- Provides a shared `harness-lib.mjs` layer for connecting, timing out, reporting failures, and keeping script behavior consistent.
- Helps validate custom server implementations and plugin flows without manually joining from a game client.

## Repository Layout

- `minecraft-ctf-bot-scripts/` - bot scripts aimed at Minecraft CTF gameplay and server checks.
- `minecraft-smoke-bot-scripts/` - Java Edition, Bedrock, online-mode, and offline/local smoke runners.
- `harness-lib.mjs` - shared Node.js harness helpers used by the scripts.
- `package.json` - Node.js workspace metadata and runtime dependencies.

## Status

This is a developer automation repo. It is intended for testing and smoke validation around Minecraft server projects, not as a standalone gameplay plugin.
