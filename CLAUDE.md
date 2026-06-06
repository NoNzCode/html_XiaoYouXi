# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML game called "鱼缸的动物们" (Animals in the Aquarium) — a tower defense game themed around an aquarium, inspired by Plants vs. Zombies.

- **Main file**: `XiaoZhangYuShengBaoBao_V1.html` — Complete game in one HTML file with embedded CSS and JavaScript
- **Design doc**: `Html 游戏简介.md` — Detailed game design specification

## Running the Game

Open `XiaoZhangYuShengBaoBao_V1.html` directly in any modern browser. No build step required.

## Architecture

The game uses HTML5 Canvas for rendering with a single self-executing function:

- **Rendering**: 60fps animation loop via `requestAnimationFrame`
- **Input**: Unified mouse/touch event handling for drag and click interactions
- **Game mechanics**: 5-lane tower defense with defender fish types (小丑鱼, 神仙鱼, 斗鱼, 清道夫) and enemy pests (蜗牛, 水蚤, 海星)
- **Auto-movement**: Idle animations when no user input
- **UI**: Bottom card selection bar, top resource display, side panels

## Key Game Constants

- Canvas size: 650x650px (scales responsively)
- Octopus head radius: 128px, 8 tentacles
- 5 attack lanes (water flow channels)