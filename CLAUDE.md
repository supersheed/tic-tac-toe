# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-file browser Tic Tac Toe game. No build system, no dependencies, no package manager — everything is plain HTML, CSS, and JavaScript in `tictactoe.html`.

## Running the Game

Open the file directly in a browser:

```bash
start tictactoe.html   # Windows
open tictactoe.html    # macOS
```

## Git & GitHub

All changes should be committed with clear messages and pushed to GitHub (`supersheed/tic-tac-toe`) to maintain a version history.

## Architecture

Everything lives in `tictactoe.html` as a single self-contained file:

- **CSS** (inline `<style>`) — dark theme, grid layout, animations
- **HTML** — 3×3 board (`div.cell[data-i]`), score boxes, status line, reset button
- **JS** (inline `<script>`) — game state (`board[]`, `current`, `gameOver`), win detection via `WINS` constant (8 lines), score tracking across games

Key logic: `checkWinner()` iterates `WINS` after every move; `init()` resets board state and DOM without reloading the page.
