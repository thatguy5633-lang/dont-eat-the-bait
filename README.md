# Don't Eat the Bait!

A third-person, up-to-8-player fishing game. The game is `index.html` plus `simple_guy_b64.js` (the character model, embedded so it also works when you double-click the file).

- Catch 31 species. Each one fights back with its own mini-game.
- Eat your catch, if you dare. Every fish gives a different effect, and the Fish Dictionary only reveals it after you've tried one.
- Level up, buy rods, bait and skills at Fin's Fish Market, and complete the dictionary.
- **Megas:** 34 kinds (every map has its own exclusive Megas), incredibly rare (a starter rod almost never hooks one). Some are fishing Megas (cast while riding) and some seat two riders giant sea creatures (about 1 in a few hundred bites in deep water; Mega Lure bait makes them ~30x likelier). Name them, feed them, level them up, recolor them, pick a swim trail, and ride them across the sea (`G`). Manage them in the Mega Stable (`M`).
- **Lava World ($100,000) and Lightning World ($500,000):** buy them at the market, then step on the glowing portal at the end of the pier to warp there. Lava World has a volcano and fire fish; Lightning World has a permanent thunderstorm, an electric sea and the best fish in the game, including Mythic ones.
- **Map expansion:** buy new areas at the market's Map tab (Outer Dock, Treasure Island, Mega Cove). Some can only be reached on a Mega.
- Dress your character in the Closet (`C`).

## Play
- **Locally:** double-click `index.html`. It needs internet because Three.js and the MQTT client load from CDNs.
- **GitHub Pages:** push this folder to a repo, then Settings → Pages → deploy from the `main` branch root.

## Online rooms
Click **Host online room** and share the 4-letter code. Friends click **Join room** and type it in. Rooms are relayed through free public MQTT brokers over secure WebSockets (EMQX / HiveMQ), so they work on home, school and most office networks without any WebRTC. Crabs, the beach ball, kicks and shoves are shared with everyone in the room. Pause (Esc) → Main menu → Leave room to exit a room.

## Extra fun (and challenge)
- **Difficulty:** Chill, Normal, Hard or Insane (title screen or pause menu). Harder modes mean tougher fights, snappier lines, a shorter hook window, more chaos and rarer BOSS fish, but more cash and XP.
- **Boss fish** (👹): rare, huge, angry fish worth 5x.
- **Buried treasure:** buy a Shovel ($250, Bait tab), follow the hot/cold hint and press N on sand to dig up chests.
- **Fin's quests**, a **cannon** and **bounce pads** on the beach, **emotes** (V), **combos**, and more chaos events (meteors, low gravity, party time).

## Phones and tablets
The game detects touch screens automatically: left thumb stick to move, drag the view to look, big 🎣 button to cast or hold to reel, plus jump, eat, kick, shove, Mega, boost and menu buttons. Tap the bottom bar to pick your rod or a fish. Landscape works best.

## Controls
| Input | Action |
|---|---|
| WASD / mouse | move / look |
| Hold LMB | charge a cast, release to throw. Click to hook a bite. |
| RMB | reel in |
| E | eat the selected fish (not the bait!) |
| Q / wheel | pick a fish in your bucket |
| 1 = rod, 2-9 = fish | pick your rod or a fish. A selected fish stays in your hands until you pick the rod again (H toggles). |
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
| Enter | text chat (online rooms) |
| Esc | pause |

Progress is saved in `localStorage`.

## Credits
Character model "Simple Guy" by jpraptor001 (https://sketchfab.com/3d-models/simple-guy-dff46ae295684c37a4860f1b374cd4ef), under the Sketchfab Standard license. Check that license before publishing the model file (`simple_guy.glb` / `simple_guy_b64.js`) publicly.
