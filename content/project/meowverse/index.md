---
title: 'Meowverse'
summary: 'An iPhone & iPad app that lets your photos grow into your cat’s little world.'
date: '2026-11-14'
tags:
  - iOS
  - SwiftUI
  - RealityKit
  - Side Project

image:
  caption: 'Development-build screenshots (iOS simulator, Nov. 15, 2026); some screens may not be in the current TestFlight build yet.'
  focal_point: Center

links:
  - name: TestFlight beta
    url: 'https://testflight.apple.com/join/WCuPQFsm'
  - name: Web demo
    url: 'https://fengyee.github.io/meowverse/'
  - name: Source (core)
    url: 'https://github.com/Fengyee/meowverse-core'

# Homepage "Outside the lab" card (layouts/partials/blox/academic-home.html)
home_kicker: 'iPhone & iPad app · side project'
home_tagline: 'Let your photos grow into your cat’s little world.'
home_meta: 'Shipped to TestFlight · Swift 6 · SwiftUI · RealityKit · 344 core-library tests'
home_screens:
  - screen-room.jpg
  - screen-memories.jpg
---

**Meowverse** turns a growing pile of cat photos into a small room your cat lives in. File photos into the furniture your cat actually uses, such as the sofa it naps on or the sunny windowsill, and tap that piece later to revisit them. You can also rearrange the room, play with your cat using a feather wand, or keep a pixel cat on your Lock Screen.

- **Native iOS and iPadOS 18+ app.** Swift 6, a SwiftUI interface, and a RealityKit renderer; English and Simplified Chinese.
- **On-device suggestions, your final say.** Apple's Vision framework suggests furniture from a preset catalog on your device; you confirm every choice. It is not photo-to-3D reconstruction.
- **Now in beta.** TestFlight build 0.1.0 (3), November 2026. A [web demo](https://fengyee.github.io/meowverse/) shows the earlier feature set.
- **Source-available core.** The [MeowverseCore](https://github.com/Fengyee/meowverse-core) library (data model, photo handling, catalog and grid rules, persistence, backup validation) is public under the PolyForm Noncommercial License 1.0.0, with 344 passing tests.
- **Built with AI coding agents.** I set the product direction and ship the releases; Claude (Anthropic) and Codex (OpenAI) helped with code and documentation. Creative ideas by Omucat.

<small>Screenshots come from a development build on the iOS simulator; the in-app photo is a synthetic sample. The in-app cat is adapted from an early template, [“3d modelling my cat: Fripouille”](https://sketchfab.com/3d-models/3d-modelling-my-cat-fripouille-0ab14bf98e754f8d90fe1bf1c84ca66c) by guillaume bolis (2020), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Full notes: [attribution](https://github.com/Fengyee/meowverse-core/blob/main/docs/media/ATTRIBUTION.md). Screenshots and app icon © Meowverse, all rights reserved; they are not covered by this site's license.</small>
