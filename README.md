# Low Tide

An independent, original card game inspired by Skyjo, made for the [Kata Arcade](https://intrepion.github.io/). No affiliation with Magilano. One human plays against two computer opponents.

## Play

Run `npm start` and visit http://127.0.0.1:8000. Run rules tests with `npm test`. The game uses static HTML, CSS, and JavaScript; a 3D library was unnecessary for this tabletop interface.

## Rules

The [original English rules](https://cdn.shopify.com/s/files/1/0019/1696/0881/files/SKYJO.pdf?v=1739260165) describe 2–8 players. Each player arranges 12 face-down cards in four columns of three and reveals two. The highest initial sum starts. Take the top discard and swap it with any card, or draw blindly and swap it or discard it and reveal a hidden card. A column of three identical visible cards is discarded. The first player to reveal all cards triggers one last turn for everyone else. Reveal remaining cards, clear matching columns, and score their sum. A finisher with a positive score that is not strictly lower than every other player's doubles it. The finisher starts the next round. When someone reaches 100 cumulative points, the lowest total wins.

This adaptation uses three players (one human and two bots), automatically resolves columns and scoring, breaks initial ties by seat order, and reshuffles all but the top discard if the draw pile runs out. These last two choices resolve situations not specified by the cited English rules. Bot decisions are an implementation choice. Original assets and presentation are used.
