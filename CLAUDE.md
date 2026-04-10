# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About Me

I build agents and skills that automate everyday routine tasks. My focus is on increasing productivity through automated, programmatic solutions that eliminate repetitive manual work — turning mundane workflows into hands-off processes.

## Project Overview

This is my Agent workspace. I use it for research, content creation and productivity workflows. 

## Rules
- Always ask for clarification if you are not sure about the task.
- Always provide a plan of action before executing the task.
- Always provide a list of tools that can be used to complete the task.
- Keep reports and summaries concise and to the point.
- Use bullet points over paragraphs
- Save all output files to the output folder
- Cite sources when doing research
- Always provide a summary of the task after it is complete.
- Always provide a feedback on the task after it is complete.
- Always provide a score on the task after it is complete.


## Running the Game

Open the file directly in a browser:

```bash
start tictactoe.html   # Windows
open tictactoe.html    # macOS
```

## Git & GitHub

Commit and push to GitHub (`supersheed/tic-tac-toe`) regularly throughout work — after each meaningful change, not just at the end. This ensures progress is never lost and any state can be reverted to. Use concise, descriptive commit messages that reflect what changed and why.

## Architecture

Everything lives in `tictactoe.html` as a single self-contained file:

- **CSS** (inline `<style>`) — dark theme, grid layout, animations
- **HTML** — 3×3 board (`div.cell[data-i]`), score boxes, status line, reset button
- **JS** (inline `<script>`) — game state (`board[]`, `current`, `gameOver`), win detection via `WINS` constant (8 lines), score tracking across games

Key logic: `checkWinner()` iterates `WINS` after every move; `init()` resets board state and DOM without reloading the page.
