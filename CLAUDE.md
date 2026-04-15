# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Running the project

No build step. Open `tictactoe.html` directly in a browser:

```bash
open tictactoe.html
```

## Architecture

Everything lives in a single file: `tictactoe.html` (HTML + CSS + JS, no dependencies).

**State**
- `board` — 9-element array (`''`, `'X'`, or `'O'`)
- `current` — whose turn it is (`'X'` or `'O'`)
- `vsCPU` — boolean toggling game mode
- `score` — `{ X, O, draw }` persisted across rounds

**Key functions**
- `handleClick(i)` — entry point for a human move; calls `place()`, then checks for win/draw, then triggers CPU if needed
- `place(i, player)` — writes to `board[]` and updates the DOM cell
- `checkWinner()` — tests all 8 winning triples; returns `{ winner, line }` or `{ winner: 'draw' }` or `null`
- `cpuMove()` — calls `minimax()` to find the best move, then delegates to `handleClick` flow
- `minimax(b, player, depth)` — recursive minimax; scores terminal states as `±(10 - depth)` so shallower wins are preferred

## Git workflow

After every meaningful change — new feature, bug fix, refactor — commit and push to `origin/main` (https://github.com/lukaskulhavy/tic-tac-toe). Never batch unrelated changes. This keeps a clean history and ensures work is never lost.

Commit message format:
- Subject line: short imperative summary (e.g. `Fix win detection for draw state`)
- Body (optional): explain *why*, not just *what*
- Always append: `Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>`

Push immediately after each commit so GitHub always reflects the latest state.
