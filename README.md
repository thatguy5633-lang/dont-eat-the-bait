# Don't Eat the Bait!

A third-person, up-to-8-player fishing game. The game is `index.html` plus `simple_guy_b64.js` (the character model, embedded so it also works when you double-click the file).

- Catch 31 species. Each one fights back with its own mini-game.
- Eat your catch, if you dare. Every fish gives a different effect, and the Fish Dictionary only reveals it after you've tried one.
- Level up, buy rods, bait and skills at Fin's Fish Market, and complete the dictionary.
- **Megas:** 34 kinds (every map has its own exclusive Megas), incredibly rare (a starter rod almost never hooks one). Some are fishing Megas (cast while riding) and some seat two riders giant sea creatures (about 1 in a few hundred bites in deep water; Mega Lure bait makes them ~30x likelier). Name them, feed them, level them up, recolor them, pick a swim trail, and ride them across the sea (`G`). Manage them in the Mega Stable (`M`).
- **Lava World ($100,000) and Lightning World ($500,000):** buy them at the market, then step on the glowing portal at the end of the pier to warp there. Lava World has a volcano and fire fish; Lightning World has a permanent thunderstorm, an electric sea and the best fish in the game, including Mythic ones.
- **Four late-game worlds, each unlocked only after the one before:** Frost World ($1,500,000, after Lightning World), Toxic World ($4,000,000), Cosmic World ($10,000,000) and The Abyss ($25,000,000). Each has its own look, 6 super-hard fish, 3 Megas and a portal at the dock of the previous world. Fish there bite slower. Catch every fish in the game to become a Master Angler.
- **The giant sea:** the ocean is about 10,000 steps across. Sail to 70+ islands (tropic, jungle, snow, volcano and rock), discover them for cash, dig their treasure with a shovel, find secret caves, fish the whirlpools, shipwrecks, reefs, kelp forests and fish schools, and pick up message bottles that hint where to look. The worlds (Lava, Lightning, Frost, Toxic, Cosmic, Abyss) sit thousands of steps out. Press `P` for the world map and a free warp back to the pier.
- **Boats** (Mega tab at the market): Row Boat, Speedboat, Sail Yacht and Hover Ship. Fast, you can fish from them, they never get hungry.
- **Mega charms:** equip them in the Stable (`M`): Land Walker (your Mega walks on land), Angler Saddle (fish while riding any Mega), Swift, Leap, Lucky and Buddy Seat. Buy them, or find them in bottles, island chests and secret caves.
- **Alive Megas:** fins and flippers flap, tails swish faster the faster you go, they barrel-roll when they leap, and a Mega waiting for you hops out of the water now and then.
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

- **Daily streak:** play on consecutive days to claim bigger gifts each day (money, bait, Mega Lures), with extra-big ones on days 3, 7, 14 and 30. Miss a day and it resets.
- **Friends:** main menu → 👥 Friends. Share your 6-character friend code, add friends' codes, see who is online, and tap Join to hop into their room.
- **Accounts:** main menu → 🔑 Sign in. Create a username and password and your whole game (fish, money, Megas, friends) saves online, encrypted with your password, so you can sign in from any device.
- **Animations:** your face now changes (happy, panic, hot, cold, sad, dizzy, sleepy, chewing, yawning, straining), you juggle a too-hot rod like a hot potato, shiver in the cold, fan yourself in the heat, cheer, flail when shoved, stretch when idle. Gulls wheel overhead and fish leap out of the sea.
- **Unique Megas:** about 30 Megas were rebuilt with their own bodies (hammerhead, jellyfish, puffer, sunfish, mantas, squid, eels, whales...). Some were renamed to match.
- **One look for the whole game:** a warm, moody, cinematic style.
- **Rods:** you can always switch to a worse rod you own (market Rod tab, or `[` and `]` in game).
- **Warm ocean:** clear turquoise shallows, bright teal water and foam where it meets the sand. Walk straight into the sea from any beach and glide into a swim. Hopping off a Mega drops you right into the water. Jumping, falling and landing have their own animations.
- **Coral reefs and ripples:** colorful coral gardens and swaying sea grass grow in the clear shallows around the islands. The sea has animated ripples, sparkles and expanding rings when you swim.
- **Underwater world:** the ONLY way down is a Sea Scooter (Fin's market, Sea Scooters tab): ride it with `G`, hold `Z` to dive and `Space` to rise. Scooters have endless air. Coral reefs only start in deeper water and grow in as it gets deeper. The water is see-through everywhere, with light shafts, plankton, schools of fish and big fish swimming around.
- **Earl's Spear Shack:** a shop on the sea floor near the pier (look for the red buoy; it's on the map too). Press `F` near Earl to buy spears and spear guns (7 tiers), the Turbo Scooter, or to sell fish.
- **Spear fishing:** underwater, hold the mouse button to aim (the ring tightens), release to fire. You can always use a worse gun you own.
- **Dev account:** open the game with `?dev=1` (for example `index.html?dev=1`) for a separate save with everything unlocked, plus a dev panel (press the backtick key) with teleports and cheats.
- **Shop categories:** Fin's market now has separate Boats (very expensive), Sea Scooters and Charms tabs.
