# Minimisation

A mobile-first web app for the Minimisation card game.

## Rules implemented
- 2–6 players.
- Standard 52-card deck, no jokers.
- Each player receives 7 cards; the starter receives 8 and discards exactly 1 before anyone picks.
- On a normal turn, the player must throw first, then pick exactly 1 card from either the immediate previous player's throw or the blind deck.
- After picking, throw either 1 card or a valid pair, triplet, quad, or same-suit consecutive sequence of 3+ cards.
- Thrown cards leave the player's hand permanently, so the objective is to minimise both remaining card count and remaining card value.
- Ace is 1 and can only be low in a sequence (A-2-3 is valid; Q-K-A is not).
- J/Q/K are worth 10.
- SHOW is available only at the start of the active player's turn, before throwing.
- SHOW scores the cards still in each player's hand; the lowest remaining total(s) score 0.
- A caller who is not tied for lowest receives their remaining total + 50.

## Current build
The app supports **2–6 players** in both pass-and-play local mode and online mode. Online mode uses PeerJS with the host browser acting as the authoritative game session; the host must keep the browser open. No persistent backend is used.

## Run locally
Open `index.html` in a browser. The online mode loads PeerJS from its CDN; local mode requires no app installation.
