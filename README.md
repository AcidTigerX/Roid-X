# Roid X

Roid X is a space shooter game built with HTML5 Canvas and JavaScript. Navigate your ship through asteroid fields, battle enemy ships, collect power-ups, and rack up your score in this action-packed arcade-style experience!

## Overview

- **Concept:** AcidTigerX
- **Developed by:** Grok (xAI)
- **Version:** 0.5 Alpha
- **Date:** February 23, 2025 (current development date)

This game features a player-controlled spaceship with advanced movement mechanics, enemy AI, asteroid physics, and a variety of power-ups to enhance gameplay. It’s designed as a single HTML file with inline CSS and JavaScript, making it easy to run in any modern browser.

## Features

- **Player Mechanics:**
  - Rotate (A/D), thrust forward (W), reverse (S), strafe (Q/E), and shoot (Space).
  - Shields (inner and optional second shield) protect against damage.
- **Enemies:**
  - Enemy ships spawn with shields at higher levels; shielded enemies bounce off a shielded player, while unshielded ones are destroyed on contact.
- **Asteroids:**
  - Normal and gold asteroids with varying sizes and hit points.
  - Gold asteroids recharge shields and award bonus points.
- **Power-Ups:**
  - Gold attraction, tri-shot, second shield, repulsion, shield recharge, EMP, faster fire, large repel, bullet wrap, and heat-seeking bullets.
- **Scoring:**
  - Earn money by destroying asteroids and enemies; lose lives and money on death.
- **Levels:**
  - Progress through 10 levels with increasing difficulty and enemy spawns.
- **Debug Mode:**
  - Toggle with 'H' to see hitboxes and test power-ups (1-5, 7-9, 0).

## Setup Instructions

### Running Locally
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/<your-username>/RoidX.git
   cd RoidX
2.Host the Files:
        Use a local server (e.g., VS Code Live Server, or python -m http.server 8000).
        Open index.html in a browser via http://localhost:8000 (direct file opening may fail due to CORS).
3. Assets:
        Ensure the assets/ folder contains all required images (listed below).
        Missing assets will cause errors or blank visuals.

Running on GitHub Pages

    Deploy:
        Push the repo to GitHub.
        Go to Settings > Pages, set the source to "main" branch, "/ (root)" folder.
    Access:
        Visit https://<your-username>.github.io/RoidX/ after deployment.

Required Assets

Place these in an assets/ folder in the root directory:

    player_ship_1.png
    asteroid_1.png to asteroid_10.png
    gold_asteroid_1.png to gold_asteroid_3.png
    enemy_ship_1.png to enemy_ship_4.png
    bullet.png
    power_up.png

Note: If assets are unavailable, replace image sources with hosted URLs (e.g., Imgur links).
Controls

    Movement:
        A: Rotate left
        D: Rotate right
        W: Thrust forward
        S: Thrust reverse
        Q: Strafe left
        E: Strafe right
    Combat:
        Space: Shoot
    Debug:
        H: Toggle debug mode (shows hitboxes)
        1-5, 7-9, 0: Toggle power-ups (when earned or in debug mode)

Game Mechanics

    Shields:
        Inner shield (7 HP) and optional second shield (7 HP) absorb damage.
        Player dies only when both shields are depleted.
    Enemy Collision:
        Shielded player vs. shielded enemy: Enemy bounces off, player shield takes 1 damage.
        Shielded player vs. unshielded enemy: Enemy destroyed, player shield takes 1 damage.
        Unshielded player vs. shielded enemy: Player dies.
    Asteroids:
        Large asteroids (75% or 100% scale) split into smaller ones and a gold asteroid when destroyed.
        Small asteroids (25% scale) despawn after 5 seconds.
    Power-Ups:
        Collectible items enhance gameplay; some can be jammed by enemies and unjammed by special power-ups.

Development

    Version History:
        0.5 Alpha: Added enemy shield collision mechanics (bounce/destroy).
        0.4 Alpha: Added strafing (Q/E), explicit thrust flags (W/S).
        0.3 Alpha: Initial release with core mechanics.
    To-Do:
        Add sound effects.
        Optimize performance for higher asteroid counts.
        Implement a main menu.

Credits

    AcidTigerX: Original concept and ideas.
    Grok (xAI): Code implementation and development assistance.

Contributions and feedback are welcome! Feel free to fork, submit pull requests, or open issues.
