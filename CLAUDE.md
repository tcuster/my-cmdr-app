# Game Companion App

## What this is
A Flutter mobile app that helps two players keep track of a long-running tabletop game's state: values, turns, steps, and triggered effects. It should feel fanciful and fun, never like a remedial aid. Players of every experience level should enjoy using it.

## The one rule that shapes everything
The app highlights; the players decide. When a trigger's condition is met, the app shows it clearly so it isn't missed. It never applies an effect, enforces a rule, or settles a dispute.

## Trigger patterns to support
- If X, then do Y
- Whenever X, do Y
- At this step, do X
- After this step, if X then Y, else Z

## Experience principles
- Companion, not tutor: friendly, in-world tone; never corrective.
- State is always visible; hints appear only when invited.
- Animations mark real moments and never slow play down.
- Every common action is one tap.
- No "beginner mode" label.

## Tech
- Flutter, Dart, Riverpod for state.
- Works fully offline; game saved on the device.
- Game-specific details (steps, values, triggers) live in config, not in core logic.
- Triggers come from card data, mapped to the four patterns; players pick cards rather than typing triggers.

## How to work with me
- I'm a solo engineer learning Claude Code on this project.
- Work on one build step at a time. Propose a short plan before writing code.
- Write unit tests for game logic before or alongside the code.
- Keep commits small, one idea each.
- Ask before adding a new package.
- Explain non-obvious choices in a sentence or two.

## Out of scope for the MVP
Automatic rule resolution, card scanning, online play, accounts, cloud sync, monetization.

## Build plan
1. Project setup
2. Game state model
3. Turn and step engine
4. Undo
5. Two-player dashboard
6. Trigger model
7. Trigger highlights
8. Loading triggers from card data
9. Fanciful layer
10. Save, resume and first playtest

Current step: 1