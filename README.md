# Age Up Coach (formerly AoE4 Helper)

A practice overlay for **Age of Empires IV** by MicroMindsGG. It reads your screen like a second pair of eyes and tells you what you missed: a build order that follows your villagers, an idle Town Center, idle villagers, and who your opponents are before the first fight.

It never reads the game's memory and never sends inputs. In a match it reads your screen only.

> **Safe? Allowed?** It only looks at your own screen - never the game's memory or files, never key presses or
> clicks, no ads or trackers (only anonymous usage counts you can switch off). Windows shows a blue "Windows protected your PC" box because the file isn't code-signed:
> click **More info → Run anyway**. There is no official ruling on overlays like this; Ranked-safe mode switches all
> screen reading off. **Everything it reads and sends, and the full answer: [TRUST.md](TRUST.md).**

**Download:** the latest `AoE4Helper-vXX.X.exe` under [Releases](../../releases). One file, no install (the spoken build steps download per build when you pick one). (The file is still called `AoE4Helper-vXX.X.exe` so updates keep working.)

## What it does

- **Build order card** with a timer that follows your villager count, step by step, with your pace against the plan. Import any aoe4guides.com build, or make your own in the editor.
- **Economy alerts:** TC idle, idle villagers, house soon / housed, too many resources banked, "you can age up".
- **Opponents:** at match start, who they are (from their public AoE4World games), how they usually play, when they attack, what they build and what beats it. `Ctrl+Alt+C` in game for the matchup.
- **Game panel:** everything the overlay shows can live inside the app window instead, so nothing pops up over your game. Only real alerts (housed, enemy in your base, TC idle) show on the game.
- **After the game:** a review with a grade, your game in three parts, an AI review from Lamporo, your villager and bank curves, every alert with its reason, and the build timeline. One goal to work on for your next 3 games.
- **Train:** hotkey drills in your own AoE4 key layout (Hotkey Coach add-on, open-source key reader: [hotkey-reader](hotkey-reader)).
- **Battle simulator** (beta): two armies, any civ and age, with the counter table.
- **Arrange on screen:** drag and resize every part of the overlay, full screen.
- **Ask AI:** ask Lamporo about the game or the app, typed or out loud.

Optional, separate download: a **map add-on** (beta) with minimap tools, for practice games. It runs on your normal key.

## Install

1. Download the `.exe` from Releases and put it anywhere (your Desktop is fine).
2. Double-click it. Windows will say **"Windows protected your PC"** - after every update, because the file isn't code-signed: click **More info → Run anyway**. Why, and how to check the file: [TRUST.md](TRUST.md).
3. Get a free key from the link in the app (one key per PC), paste it in, and follow the 2-minute setup: it finds your minimap and villager panel by itself.

Needs Windows 10 or 11 and the game at 1920×1080 or 2560×1440. Settings live in `%LOCALAPPDATA%\AoE4Helper`, so a new version never loses them.

## Free for now

Age Up Coach is free while it grows. A key is needed from the first start so that, when paid plans come, nothing changes on your side except the key. There is no end date; it will be announced on the Discord first.

## Feedback and bugs

Discord: https://discord.gg/q2ttkw5xXZ · Feedback form from inside the app (Help page).
Every alert is kept with its reason under Home → Last alerts, so "it pinged wrongly at 12:40" is enough for a bug report.

## Privacy

Age Up Coach sends anonymous usage numbers to help us improve it: which features and settings are used, how long sessions last, and basic app and Windows details (version, screen size). It never sends game content, player names, chat or AI text, key presses, screenshots or your licence key. Switch it off any time in Settings → App → "Share anonymous usage stats".

## Game content notice

Age of Empires IV © Microsoft Corporation. Age Up Coach was created under Microsoft's [Game Content Usage Rules](https://www.xbox.com/en-US/developers/rules) using assets from Age of Empires IV, and it is not endorsed by or affiliated with Microsoft.
