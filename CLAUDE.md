# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a GitHub profile README repository (`kuziyev-sharofiddin/kuziyev-sharofiddin`). It displays a personal greeting and an animated snake contribution graph on the GitHub profile page.

## Architecture

- **README.md** — Profile page content displayed on GitHub. Uses `<picture>` element for dark/light theme support.
- **.github/workflows/snake.yml** — GitHub Actions workflow that generates snake SVG animations every 6 hours using `Platane/snk@v3`, then publishes to the `output` branch via `crazy-max/ghaction-github-pages`.

## Key Details

- Snake SVGs are served via jsDelivr CDN (`cdn.jsdelivr.net/gh/kuziyev-sharofiddin/kuziyev-sharofiddin@output/...`) rather than raw GitHub URLs, for reliability.
- The `output` branch is auto-generated — do not manually edit it.
- The workflow can be triggered manually via `workflow_dispatch`.
- README content is in Uzbek.
