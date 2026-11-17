# Arena

A small first-person duel game that runs in the browser. You against a bot, first to five rounds.

Play it at https://arena.ajith.ai

- Plain WebGL, no libraries, no build step, no tracking.
- Static files on GitHub Pages: `index.html`, `arena.css`, `game.js` and a copy of the site styles and fonts in `assets/`.
- Needs a keyboard and mouse.

## Hosting

- GitHub Pages from the `main` branch root. `CNAME` holds `arena.ajith.ai`.
- DNS: `arena` CNAME to `ajithjoseph.github.io` in Cloudflare, DNS only (not proxied).
- The repo has the `ajith-app` topic, so it shows up in the app list on [ajith.ai](https://ajith.ai).

## Shutting it down

1. Remove the `ajith-app` topic, or archive the repo. It drops off ajith.ai on the next daily refresh.
2. Delete the `arena` DNS record in Cloudflare. Do this every time. A record that points at a dead Pages site can be taken over.
