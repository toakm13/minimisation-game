# Minimisation

A mobile-first web MVP for the Minimisation card game.

## Rules implemented
- 3–6 players.
- Standard 52-card deck, no jokers.
- Each player receives 7 cards; the starter receives 8 and discards exactly 1 before anyone picks.
- On a normal turn, pick exactly 1 card from either the exposed discard or the blind deck.
- After picking, throw either 1 card or a valid pair, triplet, quad, or same-suit consecutive sequence of 3+ cards.
- Thrown cards leave the player's hand permanently, so the objective is to minimise both remaining card count and remaining card value.
- Ace is 1 and can only be low in a sequence (A-2-3 is valid; Q-K-A is not).
- J/Q/K are worth 10.
- SHOW scores the cards still in each player's hand; the lowest remaining total(s) score 0.
- A caller who is not tied for lowest receives their remaining total + 50.

## Current build
This repository contains a playable **pass-and-play MVP**. It deliberately does not pretend to have online networking yet. The next production step is an authoritative realtime room server (WebSocket/Socket.IO or equivalent) plus persistent room links.

## Run locally
Open `index.html` in a browser. No npm dependencies are required.
