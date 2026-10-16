<div align="center">

# BesideAI

**One AI copilot in your browser sidebar, instead of a dozen extensions.**

Chat with the page you are on, translate meetings live, talk to your PDFs, record your screen and write email faster, all without leaving the tab.

[Website](https://besideai.work) · [Contact](mailto:contact@besideai.work)

![Manifest V3](https://img.shields.io/badge/Chrome-Manifest%20V3-4285F4?logo=googlechrome&logoColor=white)
![React](https://img.shields.io/badge/React-TypeScript-61DAFB?logo=react&logoColor=black)
![Cloudflare](https://img.shields.io/badge/Powered%20by-Cloudflare-F38020?logo=cloudflare&logoColor=white)
![Status](https://img.shields.io/badge/status-pre--release-orange)

</div>

## What is BesideAI?

BesideAI is a Chrome extension that opens as a side panel next to whatever you are working on. It combines the tools people usually install separately (an AI chat, a meeting translator, a PDF reader, a screen recorder, a screenshot tool and an email assistant) into a single, consistent product with one account.

## Features

| Feature | What it does |
|---|---|
| **Real-time meeting translation** | Live subtitles for Google Meet, Microsoft Teams and Zoom in 30+ languages. |
| **Chat with PDF** | Summarize a document, ask questions about it and extract key points. |
| **Smart AI chat** | Context-aware assistant that reads the page you are viewing. |
| **Screen recording** | Record your screen with an optional webcam overlay and share it with a link. |
| **Web capture** | Full-page or partial screenshots with annotation and sharing. |
| **Gmail assistant** | Draft emails, suggest replies and summarize long threads inside Gmail. |

## Architecture at a glance

- **Client:** Chrome Extension (Manifest V3) built with WXT, React, TypeScript, Zustand and Tailwind CSS. UI runs in the side panel; long-running logic lives in a background service worker.
- **Edge and storage:** Cloudflare Workers (including text-to-speech), R2 object storage for recordings and uploads, and Cloudflare DNS and Tunnel in front of the API.
- **AI layer:** a router that selects models by mode (speed or quality) across multiple providers.
- **Privacy by design:** permissions are scoped to what each feature needs.

## Status and roadmap

BesideAI is a bootstrapped, actively developed product in pre-release. The source code is private; this repository is the public home for product information.

Near-term focus:
- Public Chrome Web Store release
- Expanded language coverage for meeting translation
- More AI workloads running on Cloudflare Workers AI and R2

## Contact

Founder: Lam Dương · contact@besideai.work · https://besideai.work
