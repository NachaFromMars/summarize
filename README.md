# summarize — One CLI to summarize anything

> Summarize any URL, local file, PDF, image, audio, or YouTube video from the command line. Powered by your choice of AI provider — just set the API key and go.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
summarize wraps the `summarize` CLI to distill content from URLs, files, PDFs, images, audio recordings, and YouTube videos. Pick your AI provider by setting the corresponding API key; the default model is `google/gemini-3-flash-preview`. Output length is configurable from short to xxl or a specific character count.

## Features
- **Content types** — URLs, local files, PDFs, images, audio, YouTube videos
- **Providers** — OpenAI, Anthropic, xAI, Google (set the matching API key)
- **Length control** — `--length short|medium|long|xl|xxl|<chars>`
- **YouTube mode** — `--youtube auto` for direct video summarization

## Usage / Quick Start
```bash
brew install steipete/tap/summarize

# Summarize a URL
summarize "https://example.com" --model google/gemini-3-flash-preview

# Summarize a PDF
summarize "/path/to/file.pdf"

# Summarize a YouTube video
summarize "https://youtu.be/VIDEO_ID" --youtube auto

# Control length
summarize "https://example.com" --length short
```
Set one API key: `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`, `XAI_API_KEY`, or `GEMINI_API_KEY`

## Trigger Keywords (OpenClaw)
summarize URL, summarize PDF, summarize video, YouTube summary, file summary, summarize article

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
