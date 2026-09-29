
# Endless Runner

A Unity endless-runner gameplay prototype built with C#.

## Overview

The project implements the core gameplay loop of an endless runner: continuous forward movement, obstacle avoidance, collectibles, scoring and increasing speed.

## Features

- Forward player movement.
- Horizontal lane-style movement.
- Jumping.
- Procedural ground-tile spawning.
- Obstacles and collectible coins.
- Score tracking.
- Increasing movement speed.
- Death and scene-restart flow.

## Technical Focus

- Unity
- C#
- Procedural spawning
- Gameplay state management
- Collision-based interactions
- Camera follow behaviour

## Main Scripts

- **PlayerMovement.cs** — movement, jumping, death and restart flow.
- **GroundSpawner.cs** — procedural ground-tile spawning.
- **GroundTile.cs** — obstacle and coin spawning.
- **Coin.cs** — collectible behaviour.
- **GameManager.cs** — score and speed progression.
- **CameraFollow.cs** — camera tracking.

## Gameplay Loop

    Spawn ground
        ↓
    Run forward
        ↓
    Avoid obstacles / collect coins
        ↓
    Increase score
        ↓
    Increase speed
        ↓
    Fall / collide / die
        ↓
    Restart scene

## Run Locally

1. Clone the repository.
2. Open the project with Unity.
3. Open Assets/Scenes/SampleScene.unity.
4. Press **Play**.

| Action | Key |
| --- | --- |
| Move horizontally | A / D or Arrow Keys |
| Jump | Space |

## Repository Structure

    Assets/
    ├── Prefabs/
    │   ├── Coin.prefab
    │   ├── GroundTile.prefab
    │   └── Obstacle.prefab
    ├── Scenes/
    ├── Scripts/
    └── Materials/

## Project Status

A compact gameplay prototype focused on movement, procedural spawning, collectibles, scoring and restart flow.

## License

See [LICENSE](LICENSE).
