![CS2 Flash Analytics](header.jpeg)

# CS2 Flash Efficiency Analysis

Analyzing flashbang efficiency in CS2 demo files using Python.

## What it does

Parses a CS2 `.dem` file and computes, for every flash thrown in the match:
- Did it blind an enemy, a teammate, or the thrower themselves?
- How many flashes each player threw, and how many were wasted

## Why

I have 3000+ hours in CS2 and always loved to analyze my demos. I made this 
project to learn more about python and pandas by building something I actually care about

## Key findings (single match)

Funnel from 59 flashes thrown in one match:
- 59 thrown → 50 blinded someone → 34 blinded an enemy → 15 converted to a kill
- 9 flashes blinded nobody; 16 more hit only teammates/self
- Per-player conversion rates (kill within 3s of an enemy-blinding flash) ranged widely

## Status

v1 complete: single-match flash efficiency + conversion analysis.
Next: scale across multiple demos for stable per-player rates.

## Built with

- [demoparser2](https://github.com/LaihoE/demoparser) — CS2 demo parsing
- pandas — data manipulation
- Jupyter — exploratory workflow