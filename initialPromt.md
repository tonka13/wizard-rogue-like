1. Core mechanics

Movement: how many lanes/rows, or free vertical movement? Jump only, or jump + duck/slide? Let's go with a top down scroller. 
Controls: keyboard only (arrows/WASD + spacebar)? Any mouse involvement? arrows/aswd with mouse shooting projectiles
Speed: does the game speed up over time/distance, or stay constant? costant, the power and number of enemies increase over time
Camera: does the player stay fixed while the world scrolls, or does the player actually move across a level? world scrolls, but the player can move around the screen as well.

2. Obstacles & hazards

How many obstacle types for v1? (e.g., ground spikes, flying enemies, gaps/pits) no pits, as the player won't jump. 1 or 2 imp or bat sprites as enemies.
Are they randomly generated per-run, or from a pattern pool you define? randomly generated
Fixed difficulty or ramping — do obstacles get denser/faster over time? remping with check points. The player gets to a boss where the camera stops scrolling, fights the boss, and beating give the option to purchase power ups

3. Power-ups / upgrades

In-run power-ups (temporary shield, speed boost, double-jump)? No in run power ups, they come in between bosses.
Between-run permanent upgrades (the roguelite loop) — what currency do you earn, and what does it buy? (e.g., "coins" collected during runs → permanent jump height upgrade) killing enemies grants gems you can spend after each boss. Boss gives enough gems to buy at least one upgrade even if you just dodge every enemy along the way.
How many upgrade types for v1 — 3-4 is plenty to start. 2 or 3 is good. regenerating sheild, multi attack, extra life

4. Death / permadeath rules

Instant death on hit, or a health/lives system? 3 hits is death
What happens on death — return to a menu, show a stats screen, restart immediately? show stats (how long you played, how many enemies killed, how many bosses killed) then return to menu
Does progress (currency/upgrades) persist through death, or reset? Reset for now

5. Visual style

Pixel art, flat vector shapes, or simple geometric placeholders for now (squares/circles) to get mechanics right before art? pixel art of either wizard or archer character
Palette/mood — dark and moody, bright and cartoonish, retro 8-bit? retro 8-bit dungeons and dragons vide

6. Scope guardrails for Fable

Explicitly state: "single HTML file, vanilla JS + Canvas, no external art/asset dependencies for v1" — keeps it buildable and testable immediately in browser.
Tell it what NOT to build yet (multiplayer, sound, save-to-server) so it doesn't over-engineer.

7. What "done" looks like for this session

A playable core loop: move, dodge one obstacle type, collect one power-up type, die, see a score, restart.
Everything else (more obstacle variety, upgrade shop, art polish) is a fast-follow once the loop feels fun.