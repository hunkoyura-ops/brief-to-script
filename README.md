# Brief → Script

A web tool I built to generate scripts for short-form video.

You give it a brand, a key message and a creator's style. It returns a timecoded script (hook → body → proof → CTA) with on-screen text cues, a caption and hashtags.

Live: [brief-to-script.hunkoyura.workers.dev](https://brief-to-script.hunkoyura.workers.dev/)

## Modes

- **Single**: one script for one creator.
- **Batch**: several creators in one pass.
- **Presets**: for creators you work with regularly. Their style is saved once and never typed in again.

## How it works

The tool runs on its own backend (Cloudflare Worker + Claude API). If the AI is unavailable, it automatically falls back to local templates, so a request never comes back empty.

## Stack

- Cloudflare Workers
- Anthropic Claude API

## Author

Yurii Hunko, [hunkoyura.com](https://hunkoyura.com)
