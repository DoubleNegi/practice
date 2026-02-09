# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Single-page interactive tutorial for Claude Code, written in Japanese. The entire application is a single `index.html` file containing HTML, CSS, and JavaScript with no build tools or dependencies.

## Architecture

- **index.html**: Self-contained SPA with inline `<style>` and `<script>` blocks
  - CSS custom properties (`:root` variables) control the dark theme
  - `chapters` array in JS holds all tutorial content (12 chapters across 4 levels)
  - Progress state is persisted to `localStorage` under key `claude-code-tutorial-progress`
  - Sidebar navigation, chapter rendering, and progress tracking are all vanilla JS

## Development

No build step. Open `index.html` directly in a browser to preview.
