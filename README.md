# Holiday Havoc — House Royale 🎄

A goofy free-for-all shooter set on (and inside) a real house. Snowball blasters, candy cane snipers, ornament shotguns, leaf blowers and fruitcake grenades. Timed rounds, random respawns, and whoever has the most kills when the clock hits zero wins.

## Play
Open the site, pick a name and color, hit **Play**. Send friends the link from **Copy invite link**. Everyone on the same link plays in the same match.

- `?room=yourcode` at the end of the URL gives you a private room. The **New private room** button makes one.
- The first person in a room is the host 👑 and controls round length, respawn delay, damage, gravity, speed, starting fruitcakes and time of day.

## Controls
| | |
|---|---|
| WASD | move (Shift sprint, Space jump) |
| Mouse | aim; left click shoot; right click aim/scope |
| 1 / 2 / Q / wheel | switch weapon |
| R | reload |
| G | throw fruitcake |
| E | grab gift (also automatic) |
| Tab | scoreboard |
| Esc | menu |

Phones get a joystick plus on-screen buttons.

## How multiplayer works
Players connect straight to each other's browsers (WebRTC). Public Nostr relays are only used to find each other, through the bundled [Trystero](https://github.com/dmotz/trystero) library (`trystero.js`). There's no server to run and nothing to pay for. A few very strict networks (some school/work Wi-Fi) block direct connections; most home internet and phones are fine.

## Hosting
It's just static files: `index.html`, `trystero.js`, `.nojekyll`. Put them on GitHub Pages, Netlify, Cloudflare Pages, or any static host.
