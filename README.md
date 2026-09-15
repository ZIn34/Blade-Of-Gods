# Blade of Gods

A 2D side-view action platformer that runs in a single HTML file. No build step, no
dependencies: open `cave-runner.html` in a browser and play.

You are Sir Thraine, a knight who trained among the assassins and whose father was a mage.
Monsters dragged you into the dark. You wake in a cave with nothing but your daggers.

## Play

Open `cave-runner.html` (or serve the folder and open `index.html`).

| | Keyboard / mouse | Controller |
|---|---|---|
| Move | arrows / WASD | left stick, d-pad |
| Jump | Z / Space | A |
| Attack | click or X, aimed at the mouse | RT |
| Uppercut / ground slam | aim up / aim down in the air | right stick up / down |
| Dodge roll | right click / Shift | B |
| Throw dagger | F / R | LB |
| Vanish | V / G | LT |
| Charge | C | X / RB |
| Rage smash | Q / middle click | Y |
| Stone powers | 1 / 2 / 3 / 4 / 5 | |
| Talk / use | E / Up | d-pad up |
| Map, items, skills | Tab | Back |
| Pause | Esc | Start |
| Music | M | |

## The run

1. Clear the road to the village and meet the Old Miner.
2. Kill the dragon blocking the road east.
3. Take the four elemental stones from the giant, the ice dragon, the fire dragon and the
   stone golem. Each guardian needs its own strategy; steel alone does not work on any of them.
4. Climb the cloud stair and ask the gods for the Blade of Gods. They send you after three
   raiding dragons first, and then after the giant that steals the blade out from under them.
5. Go down the pit in the deep hall, through a keep of rope-and-door puzzles, and end the mage.

Every stone becomes an ability on a hotkey. Levels past 80 grant skill points for a ten-skill tree.

## Layout

    cave-runner.html    the whole game: engine, art helpers, audio, content
    index.html          redirect, so GitHub Pages serves the game at the repo root
    sprites/            sprite sheets and source art
    sounds/             dragon fire
    music/              theme

## Saves

Three named save slots in `localStorage`, plus an autosave every five minutes. Saving is
blocked during boss fights.
