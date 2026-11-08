# Ron vs the Basilisk

**Ron vs the Basilisk** is a short first-person fan game set deep beneath Hogwarts. In his final year, Ron goes down into the flooded Chamber of Secrets alone to face a blinded, enraged basilisk, armed with only his wand and his nerve.

> Unofficial, non-commercial fan game. Not affiliated with or endorsed by the Harry Potter rights holders.

## The story

Far below the castle, the Chamber of Secrets lies open, and its ancient guardian is awake. A phoenix sweeps out of the dark and claws out the serpent's eyes. Blind and screaming, it can no longer see you. But it can still hear you.

## Gameplay

- **Incendio:** a fast stream of fire that keeps the pressure on.
- **Stupefy:** stuns the basilisk for 7 seconds and makes your attacks hit harder. It takes 15 seconds to recharge, shown by a bar on its icon.
- **Venom volleys:** the basilisk spits a wide spread of venom every 1.45 seconds, aimed at where you're about to be.
- **Rams:** once it's badly hurt, it starts charging at you. Watch for the red warning line, roll out of the way, and lure it into a pillar to daze it.

## Features

- A cinematic opening with a phoenix attack and spoken narration, and an ending cutscene when the basilisk falls
- A horned, armoured basilisk with a hide made from a real reptile-skin scan
- Venom that wobbles in flight, splashes, sizzles on the floor and spatters your view
- A flooded hall of scanned stone, with fluted serpent pillars, carved friezes, chained fire bowls, rippling water, mist and shafts of light
- Atmospheric sound: falcon cries, a growling serpent, war drums that speed up as the fight turns, and a heartbeat when you're close to death
- Automatic quality: on weaker laptops the game lowers its resolution to stay smooth
- Memory protection: the game won't start without enough free memory, and closes itself before the PC runs out

## Controls

| Key | Action |
|---|---|
| W A S D | Move |
| Mouse | Look |
| Left click | Cast (hold to keep casting) |
| Scroll | Switch between Incendio and Stupefy |
| Space + A / Space + D | Roll left / right |
| Esc | Pause (Resume, Main Menu, Quit) |
| Enter | Skip a cutscene |
| Ctrl + Shift + Q | Quit instantly, even if the game hangs |

## Install

1. Download **RonVsBasilisk-Setup.exe** from the [Releases](../../releases) page.
2. Run it. Windows may show "Windows protected your PC", because the installer isn't signed by a paid publisher. Click **More info**, then **Run anyway**.
3. Start the game from the desktop or Start menu shortcut.

To uninstall, use **Settings → Apps** in Windows.

### Requirements

- Windows 10 or 11, with Microsoft Edge (included with Windows). Nothing else to install.
- About 3 GB of free memory when starting.
- A graphics card is recommended. Integrated graphics work, at a lower resolution.

## Running from source

The game is plain HTML and JavaScript and needs no build step. Open `game/index.html` in Microsoft Edge to play it directly.

To build the installer yourself, run this in PowerShell from the repository folder. It uses the C# compiler that comes with Windows (.NET Framework 4).

```powershell
powershell -ExecutionPolicy Bypass -File installer/build.ps1
```

The installer is written to `dist/RonVsBasilisk-Setup.exe`.

## Project layout

| Folder | Contents |
|---|---|
| `game/` | The game: `index.html`, scripts in `js/`, embedded models, textures and voices in `assets/`, and three.js in `vendor/` |
| `installer/` | The Windows installer and launcher (`Setup.cs`) and its build script |
| `tools/` | Developer tools used to prepare the character and hand models. They need a local web server to run. |

## Credits

The game is built on [three.js](https://threejs.org). Third-party models, textures and voices are listed with their licences in [`game/CREDITS.txt`](game/CREDITS.txt):

- Ending characters by Grab3D (CC0)
- First-person hand from Microsoft Rocketbox (MIT)
- Phoenix by NORBERTO-3D (CC BY 4.0), recoloured
- Basilisk hide and chamber stone from ambientCG (CC0)
- Voices generated with Piper text-to-speech

## Licence

No licence is granted for this project. The original code is shared for viewing only. Third-party material keeps its own licence, as listed in `game/CREDITS.txt`. Harry Potter characters, names and places belong to their respective owners.
