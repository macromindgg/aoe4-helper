# Is Age Up Coach safe? Is it allowed?

Straight answers, from the code itself. Age Up Coach (formerly AoE4 Helper) is a practice overlay for
Age of Empires IV made by MacroMindGG.

## "Windows protected your PC" - why you see it

- That blue box is **Microsoft Defender SmartScreen**. It shows for files Windows hasn't seen on many PCs yet.
  It means *unknown*, not *dangerous*.
- Our `.exe` is **not code-signed**. For unsigned files
  Windows starts every new version from zero, so you will see the box again after each update.
- **To start it:** click **More info**, then **Run anyway**.
- **Only download it from** [github.com/macromindgg/aoe4-helper/releases](https://github.com/macromindgg/aoe4-helper/releases).
- **Check the file yourself:** each release lists the file's SHA-256. Paste it into
  [VirusTotal](https://www.virustotal.com/) or Microsoft's own [file lookup](https://www.microsoft.com/wdsi/filesubmission)
  to see every antivirus result.

## What it reads

- **Your screen.** It copies the game's picture many times a second, in memory, and looks at fixed spots: the
  villager icon, your resources and population, your age, the production queue, the player list - and the
  minimap if you installed the map add-on. Nothing is saved or sent, except what you switch on yourself
  (Auto clips are saved on your PC; a screenshot goes with "Report a problem" only if you tick it).
- **Public match data** from [aoe4world.com](https://aoe4world.com): your and your opponents' public profiles and games.
- **Keys - Hotkey Coach add-on only.** Whether the keys on a short list (your TC key, villager key, control
  groups, at most 40) are held down - only while Age of Empires IV is the active window, never while the chat is
  open. The key reader is open source (MIT): [hotkey-reader/reader.py](hotkey-reader/reader.py), about 150 lines.

## What it never does

- Never reads or changes the game's memory or files, and never injects anything into the game.
- Never sends key presses, mouse clicks or camera moves. Every build runs an automatic check that fails if code
  for that ever appears.
- Never plays for you or automates anything - it only tells you what it saw.
- No ads and no third-party tracking. The only usage numbers are the anonymous counts in the table below; they go to
  our own server and one switch turns them off.

## What leaves your PC

| What | Where to | When |
|---|---|---|
| Your key, a random install id and a label like "PC-1a2b" (a short scramble, not your PC's name) | our licence server | when the app starts |
| A short summary of a finished game (civs, names, map, times, what to fix) and the **text** of your question - never your voice | our server, then the AI (Claude by Anthropic) | only with AI Helper on; reviews are kept 3 months |
| Anonymous usage counts: which pages and features are used, how long the app runs, the app version, the kind of an error. Never names, chat or AI text, key presses, screenshots, file paths or your key | our licence server | while the app runs - off with Settings → App → *Share anonymous usage stats* |
| Per-minute numbers of finished games (no names, no game ids) | our server | only with Settings → *Help improve win chance* on (off by default) |
| An update check | GitHub | when the app starts |
| Version, settings and your last alerts (+ a screenshot if you tick it) | our support bot | only when you press "Report a problem" |
| Your match card | your Discord channel | only if you paste a Discord webhook |
| A build's notes | MyMemory (translation) | only when you press "Translate to English" |

## Is it allowed?

- **There is no official ruling.** World's Edge and Relic have not said yes or no to overlays like this, and we
  have not asked for or received approval. We won't pretend otherwise.
- **How we keep it fair:** it only looks at what is already on your own screen, never touches the game, never
  automates anything. It is a coach, not a bot.
- **Ranked-safe mode** switches all screen reading off. You can also let it switch on by itself whenever
  AoE4World reports a ranked game.
- **The map add-on** (minimap enemy pings) is a separate, optional download. It is not meant for ranked - that
  choice is yours.
- **Tournaments** often ban all third-party software. Close the app for tournament games.
- **Not sure?** Use it in practice, unranked and games against the AI.

## Questions

Ask in our Discord: [discord.gg/q2ttkw5xXZ](https://discord.gg/q2ttkw5xXZ) - or read the key reader's code yourself.
