# BesideAI

**An AI copilot that lives in your browser sidebar.** BesideAI is a Chrome extension (Manifest V3) that brings several everyday tools into one side panel, so you can chat, translate, read and record without switching tabs.

Website: https://besideai.work

## Features

- **Real-time meeting translation**: live subtitles for Google Meet, Microsoft Teams and Zoom in 30+ languages.
- **Chat with PDF**: summarize, ask questions and extract insights from PDF documents.
- **Smart AI chat**: context-aware chat that can read the page you are viewing.
- **Screen recording**: record your screen with an optional webcam overlay and get a shareable link.
- **Web capture**: take full-page or partial screenshots, annotate them and share.
- **Gmail assistant**: draft emails, suggest replies and summarize long threads inside Gmail.

## Technology

- Chrome Extension, Manifest V3, built with [WXT](https://wxt.dev), React, TypeScript, Zustand and Tailwind CSS.
- Backend and edge on [Cloudflare](https://www.cloudflare.com): Workers (including text-to-speech), R2 object storage and Cloudflare DNS/Tunnel in front of the API.
- Multi-provider AI routing with model selection by mode (speed / quality).

## Status

BesideAI is a bootstrapped, actively developed product. The source code is currently private; this repository is the public home for product information.

## Contact

contact@besideai.work
