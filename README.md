# Hive Guardian — Maltese Edition

**Alpha build · v1.0.0-alpha.1**

Produced by **BarusXXX and about 15 AI Agents**.
[kaneborg.com](https://kaneborg.com/)

## The game

Protect a Maltese honey bee colony in a flowering Mediterranean garden.
Manage the colony, build its defences and take flight as a single worker bee.
This alpha release is still being refined.

Choose **Deploy Colony**, then **First Flight** to learn the controls.
Select a defence and an empty mounting point to build it. Keep enough workers
foraging, deliver nectar and pollen, and protect the hive's entrance and brood.
Use **Take Flight** to control an individual bee in the same colony.

## Controls

| Control | Action |
| --- | --- |
| W / A / S / D | Pan in strategy view; fly or walk in bee view |
| Drag the scene | Pan in strategy view; look around in bee view |
| Mouse wheel | Zoom in strategy view |
| Q / E | Descend / ascend while hovering |
| F | Land / lift off |
| Hold G | Gather |
| H | Return cargo to the hive |
| R | Rally guards |
| Space | Pause strategy view; bite and grapple in bee view |
| X | Use the worker's one-use last sting, sacrificing that bee |
| Tab | Switch between strategy and bee view |
| T | Toggle quarter-speed slow motion |
| Escape | Pause / resume |

In flight, look up or down while moving forward to climb or dive.
On touch screens, use the flight stick, drag to look, and the altitude and action
buttons. Drag to pan and pinch to zoom in strategy view.
Phones keep compact icon controls in portrait and landscape. Health and cargo
sit in the upper corner, and the tactical map stays hidden. In strategy view,
tap the + on the colony panel to show its details and guard allocation.

## Language and age guidance

Recommended ages **16+**. The game contains stylized insect combat and death.
Bee voice options are **Off**, **Normal** and **Salty**, with Normal selected by
default. Salty includes strong Maltese language. Parental guidance is advised.
Voice volume and other audio settings are available in Options.

The field guide distinguishes practical beekeeping measures from speculative
game technology. Fictional chemistry and accelerated colony behaviour are
gameplay abstractions, not real beekeeping instructions.

## Saves and offline play

Saves are stored in the browser on the current device. Use the save controls in
Options to save, export or import a colony. Export a save before clearing browser
data or moving to another browser or device.

After the hosted game has loaded successfully and cached its files, it can be
revisited offline in the same browser. External reference and contact links
require an internet connection.

## Test the release locally

Opening `index.html` directly creates a `file://` address. Browsers block the game's
JavaScript modules at that address. Use a local web server instead.

With the source repository and its dependencies installed, run from the repository root:

```powershell
cd game
npm run preview
```

Open [http://127.0.0.1:4173/](http://127.0.0.1:4173/) in your browser. This serves the
built dist; keep the terminal running while playing.

If you have only this release folder and Python installed, open a terminal in the
folder containing `index.html` and run:

```powershell
python -m http.server 8000 --bind 127.0.0.1
```

Then open [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Hosting this release

This folder is ready for static web hosting. Upload its complete contents to an
HTTPS site, preserving the file names and directory structure. Assets load
relative to the folder containing `index.html`, so the same build works at the
site root or under a folder such as `/HiveGuardian/`.

For GitHub Pages, upload the contents of this folder to your configured Pages
publishing location, including the `.nojekyll` file. Open the published Pages URL,
such as `https://barusxxx.github.io/HiveGuardian/`. The manifest and offline cache
use that folder as their scope. Replace the complete previous release when updating.

Serve `index.html` through a web server rather than opening it as a local file.
No game backend or build tools are needed on the host. Use a browser with WebGL 2
support; select Low graphics in Options if performance is slow on your device.

## Help, localisation and feedback

Want to help with Hive Guardian or localise it for your language and setting?
[Reach out through the contact page](https://kaneborg.com/contact/).

Have a method for dealing with hornets that is not covered in the field guide?
Share it with us so we can spread the word. You can also use the contact page to
report bugs; include the game version, browser and device, and what happened.

## Licence and credits

Copyright (c) 2026 Kane Borg (BarusXXX).

Original project code and documentation are released under the [MIT licence](LICENSE).
Included third-party components and assets retain their respective licences.
See [CREDITS.md](CREDITS.md) for attribution, asset sources and the Three.js licence.
Credits are also available inside the game from the intro screen.
