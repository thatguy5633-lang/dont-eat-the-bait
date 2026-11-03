# Don't Eat the Bait!

A third-person, up-to-8-player fishing game. The game is `index.html` plus `simple_guy_b64.js` (the character model, embedded so it also works when you double-click the file).

- Catch 31 species. Each one fights back with its own mini-game.
- Eat your catch, if you dare. Every fish gives a different effect, and the Fish Dictionary only reveals it after you've tried one.
- Level up, buy rods, bait and skills at Fin's Fish Market, and complete the dictionary.
- **Megas:** incredibly rare giant sea creatures (about 1 in a few hundred bites in deep water; Mega Lure bait makes them ~30x likelier). Name them, feed them, level them up, recolor them, pick a swim trail, and ride them across the sea (`G`). Manage them in the Mega Stable (`M`).
- **Map expansion:** buy new areas at the market's Map tab (Outer Dock, Treasure Island, Mega Cove). Some can only be reached on a Mega.
- Dress your character in the Closet (`C`).

## Play
- **Locally:** double-click `index.html`. It needs internet because Three.js and the MQTT client load from CDNs.
- **GitHub Pages:** push this folder to a repo, then Settings → Pages → deploy from the `main` branch root.

## Online rooms
Click **Host online room** and share the 4-letter code. Friends click **Join room** and type it in. Rooms are relayed through free public MQTT brokers over secure WebSockets (EMQX / HiveMQ), so they work on home, school and most office networks without any WebRTC. Pause (Esc) → Main menu → Leave room to exit a room.

## Controls
| Input | Action |
|---|---|
| WASD / mouse | move / look |
| Hold LMB | charge a cast, release to throw. Click to hook a bite. |
| RMB | reel in |
| E | eat the selected fish (not the bait!) |
| Q / wheel | pick a fish in your bucket |
| R | switch bait |
| F | market (near the stall) |
| B | Fish Dictionary and skills |
| C | Closet |
| G | summon / ride / dismount your Mega |
| M | Mega Stable |
| K | kick (crabs, the beach ball...) |
| X | shove other players (push them off the dock!) |
| T | Skills (its own screen) |
| Space (in the air) | jump off the dock and swim; Space near a dock to climb out |
| Shift / Space (riding) | boost / leap |
| Esc | pause |

Progress is saved in `localStorage`.

## Credits
Character model "Simple Guy" by jpraptor001 (https://sketchfab.com/3d-models/simple-guy-dff46ae295684c37a4860f1b374cd4ef), under the Sketchfab Standard license. Check that license before publishing the model file (`simple_guy.glb` / `simple_guy_b64.js`) publicly.
