# 🏰 Tower Defense Game

Welcome to the **Tower Defense** game! Strategize, build defenses, and protect your base from waves of incoming enemies. 

You can play the game directly in your browser here:
👉 **[Play the Game on GitHub Pages](https://finkord.github.io/tower_defense_build/)**

## Towers
The game features a flexible, data-driven tower system (`TowerData.cs`). You can create various tower types by mixing standard stats and special abilities.

| Tower Name | Damage | Range | Fire Rate (shots/sec) | Price | Special Abilities |
|------------|--------|-------|-----------------------|-------|-------------------|
| **Archer** | 2 | 5.5 | 2.5 | 100 | None |
| **Cannon** | 8 | 8.5 | 0.5 | 260 | High Damage, Long Range |
| **Freezer**| 1 | 5.0 | 0.8 | 130 | **Crowd Control:** Slows enemies by 50% for 2.5s |
| **Mage**   | 2 | 4.3 | 0.6 | 200 | **Area of Effect:** Deals splash damage in a 2.8 unit radius |

## Enemies
Enemies are also data-driven (`EnemyData.cs`) and scale dynamically across waves. We use a **Dual Economy System** where the `Reward` goes to the Defender, and the `PvP Cost` is used by the Attacker's budget.

| Enemy Name | Health | Speed | Kill Reward | PvP Cost | Special Features |
|------------|--------|-------|-------------|----------|------------------|
| **Goblin** | 5 | 3.8 | 5 | 5 | Fast, squishy swarm unit |
| **Ghost**  | 8 | 2.4 | 10 | 10 | **Immune to Slow** effects (counters Freezer) |
| **Orc**    | 28 | 1.5 | 15 | 15 | Heavy Tank unit |
