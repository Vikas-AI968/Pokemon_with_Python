# Poké‑Lite — Pokémon with Python 🐾🎮

> A compact, retro‑styled Pokémon‑inspired adventure built with Pygame — fast to run, friendly to tweak, and crafted for pure nostalgic fun.

[![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/) [![Pygame](https://img.shields.io/badge/pygame-required-orange)](https://www.pygame.org/)

---

✨ Features
- Charming 2D overworld with NPCs, collisions and grass encounters.
- Turn/initiative-based battles with elemental typing (fire / water / plant).
- Monsters gain XP, level up and evolve — progression that feels rewarding.
- Modular code structure: easy to add monsters, attacks, maps and assets.
- Lightweight and beginner-friendly — perfect for learning and modding.

---

🚀 Quick Start (Windows)
1. Clone the repo and open a PowerShell / CMD in the project root.
2. Create & activate a virtual environment:
   ```powershell
   python -m venv .venv
   .venv\Scripts\activate
   ```
3. Install dependencies:
   ```powershell
   pip install pygame pytmx
   ```
4. Run the game:
   ```powershell
   python code\main.py
   ```
5. If assets are missing, ensure the repo root contains the folders: `graphics/`, `audio/`, `data/`.

---

🎮 Controls
- Arrow keys — Move the player
- Space — Interact / Advance dialogue / Confirm
- Enter — Open/close Monster Index (party screen)
- Escape — Cancel / Back
- Close window — Quit

---

🗺️ Project Layout (key files)
- code/main.py — Game loop & high-level flow
- code/settings.py — Constants, UI colours & layout
- code/sprites.py — Overworld & battle sprite classes
- code/entities.py — Player & NPC behaviour
- code/battle.py — Battle engine & UI
- code/monster.py — Monster stats, XP and evolution
- code/support.py — Asset importers & helpers
- code/timer.py — Simple timer utility
- data/ — Map TMX & JSON game data (MONSTER_DATA, ATTACK_DATA)
- graphics/, audio/ — Required media assets

---

🧭 Gameplay Overview
- Roam the map and enter patches of grass to trigger wild encounters.
- Battles revolve around initiative — monsters build initiative to take turns.
- Attacks cost energy; element matchups affect damage multipliers.
- Earn XP, level up and evolve monsters per definitions in `game_data`.

---

🛠️ Modding & Development Tips
- Add new monsters or attacks in `data/game_data.py` (MONSTER_DATA / ATTACK_DATA).
- Edit maps with Tiled; put TMX/maps into `data/` and matching tiles in `graphics/`.
- Sprite sheets are parsed by `support.py` — follow existing folder conventions.
- For faster debugging keep a terminal open to read Python tracebacks.

---

💡 Pro tips
- Lower WINDOW_WIDTH/HEIGHT in `settings.py` to improve performance.
- Missing asset errors usually mean incorrect working directory — run from repo root.
- Use your own sprite sheets but match expected frame layouts or update `support.py`.

---

🤝 Contributing
1. Fork → feature branch → PR with a focused description.
2. Include screenshots or short notes explaining behavior changes.
3. Keep assets properly licensed; attribute any third‑party content.

---

📜 License
This project is provided as‑is for learning and educational purposes only.

---

📬 Get in touch
Open an issue or PR in this repository for bugs, suggestions or contributions.

---

Have fun — code, explore and evolve your way to victory! ⚡🌿🔥
