# Chat Hoops

A Twitch chat interactive basketball overlay. Viewers throw spinning coins into a moving basket by sending messages in chat. Designed as an OBS browser source overlay.

## How to use

1. **Open the setup page** — visit `index.html` (or the GitHub Pages URL for your fork).
2. **Fill in your channel name** and choose your trigger type and background.
3. **Copy the generated URL** and paste it into OBS as a Browser Source at **1920×1080**.
4. Set the browser source background to transparent in OBS (check "Allow transparency").

### Trigger options

| Setting | Behavior |
|---|---|
| Every message | Any chat message throws a coin |
| Emotes only | Only messages containing a Twitch emote throw a coin |
| Custom command | Only messages starting with e.g. `!shoot` throw a coin |

### Background options

| Setting | URL param |
|---|---|
| Transparent (default) | *(omitted)* |
| Gradient | `bg=1` through `bg=7` |

## Controls

| Key | Action |
|---|---|
| `SPACE` | Pause / resume the game |
| `D` | Toggle debug mode (shows collision zones and coordinates) |

## Deploy your own GitHub Pages instance

1. Fork this repo on GitHub.
2. Go to **Settings → Pages** and set the source to the `main` branch, root folder.
3. Visit `https://<your-username>.github.io/<repo-name>/` to open the setup page.

No build step required — tmi.js is loaded from CDN.
