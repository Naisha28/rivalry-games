# Rivalry 🎮

Play games here: https://naisha28.github.io/rivalry-games/

**Good friends. Bad losers.**

Rivalry is a lightweight, browser-based party game collection for playing with friends — on one shared screen ("couch mode") or online in a room with an invite code. No build step, no backend: it's a single static page.

## Games

- **Trivia** – answer questions faster than your friends
- **Rock Paper Scissors** – secret picks, pass-the-screen style
- **Word** – guess the word from a clue before time runs out
- **Reaction** – tap the moment the screen flips (tap early and score 0)
- **Memory** – flip cards and match pairs

## Features

- Local multiplayer (pass the screen) and online rooms via a shareable code or invite link
- Add bot friends to fill the lobby
- Scoreboard, results screen with confetti, and one-tap rematch / switch game
- Custom 404 page

## Tech

- Vanilla HTML/CSS/JavaScript in a single file ([index.html](index.html))
- [PeerJS](https://peerjs.com/) (peer-to-peer WebRTC) for online rooms
- Google Fonts: Space Grotesk and JetBrains Mono

## Getting started

Clone the repo and serve the folder with any static server:

```bash
python3 -m http.server 5179
```

Then open <http://localhost:5179>.

Online mode needs internet access (PeerJS CDN and signaling server).

## Project structure

```
.
├── index.html   # The whole app: markup, styles, game logic
├── 404.html     # Custom "not found" page
└── README.md
```

## Deployment

Because it is fully static, it can be hosted on any static host. The `404.html` is picked up automatically.

## License

Add a license of your choice (e.g. MIT) before publishing.
