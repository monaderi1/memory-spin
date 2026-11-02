# Memory Spin

Memory Spin is a mobile-first collection of visual attention and memory games.

## Run

Open `index.html` in a modern browser. The project is a **single HTML file**: no build step, npm install or app package is needed.

## Games

- **Numbers**: find 1–50 in order on a mosaic wheel or triple rings, which may be still or spinning.
- **Categories**: memorize where items sit (numbers, fruits, animals, tools, flags or words), then find each requested one. This replaces the old separate Memory game.
- **Pattern**: repeat a drawn unlock pattern. The 20 levels choose patterns by measured difficulty (turns, crossings, knight moves, jumps over used dots), so high levels never get an easy one by chance. Higher levels also spin faster, in a random direction or chaotically, trace the preview without step numbers, and at the top ask you to draw it backwards.
- **Links**: remember the order in which numbers are connected, then reconnect them after they shuffle.
- **Recall**: reproduce a sequence forward or in reverse (digits, pictures or words).
- **Target**: find changing targets on one or more rings.
- **Split**: memorize a number such as 453278. After it hides, a split rule is revealed: plain pairs (45 32 78), each pair flipped (54 23 87) or pairs from the 2nd digit (53 27). Tap the matching pairs among traps, which include the pairs the other rules would give, reversed pairs and near numbers. Higher levels add digits, mix all rules and require the pairs in order.

## Levels and Practice

Every game has a fixed ladder of levels (9–14 per game). Each level pins all of that game's settings, so results are comparable over time.

- Each level has **one pass condition** (time, mistakes, or correct taps), shown before you start. Pass it and the next level unlocks; otherwise retry.
- After a round you see what was needed and what you did, so you know how close you were.
- **Practice** keeps the free settings under ⚙ Options. Practice rounds are saved but never count toward levels or stars.

Progress is measured as *highest level passed*. The old 0–1,000 score across mixed settings has been retired. Rounds recorded under the old scoring stay in storage and backups, but they are not charted.

When a ladder's meaning changes, its version (`LADDER_VERSION`) is raised and older rounds for that game are archived. The ladders and pass conditions are defined in `LEVEL_LADDERS` inside `index.html`. They are first estimates and should be tuned after real play-testing.

## Profiles and results

Profiles and history are stored locally in the browser. Data is not shared between different browser origins, including different local file URLs. Use **Export Backup / Import Backup** under Profiles when moving the file or changing devices.

## Notes

- The user interface is in English.
- Some recorded animal sounds need internet access; the app falls back to synthesized sounds.
- This is an experimental game project, not a clinically validated cognitive assessment or treatment.
