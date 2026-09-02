# Minimisation

A mobile-first web MVP for the Minimisation card game.

## Rules implemented
- 3–6 players.
- Standard 52-card deck, no jokers.
- Each player receives 7 cards; Player 1 starts with 8.
- On a turn, draw either the exposed discard or a blind deck card, then discard one.
- Valid combinations: pairs, triplets, quads, and same-suit consecutive sequences of 3+ cards.
- Ace is 1 and can only be low in a sequence (A-2-3 is valid; Q-K-A is not).
- J/Q/K are worth 10.
- SHOW automatically minimises each hand mathematically.
- Lowest total(s) score 0; a caller who is not tied for lowest receives their total + 50.

## Current build
This repository contains a playable **pass-and-play MVP**. It deliberately does not pretend to have online networking yet. The next production step is an authoritative realtime room server (WebSocket/Socket.IO or equivalent) plus persistent room links.

## Run locally
Open `index.html` in a browser. No npm dependencies are required.
