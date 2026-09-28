# Endless Runner

A Unity endless-runner gameplay prototype built with C#.

## Overview

The project implements the core loop of an endless runner:

- forward player movement
- horizontal lane-style movement
- jumping
- spawned ground tiles
- obstacles
- collectible coins
- score tracking
- increasing movement speed
- scene restart after the player dies

## Technical focus

**Engine:** Unity  
**Language:** C#

Key scripts:

- `PlayerMovement.cs` — movement, jump, death and restart flow
- `GroundSpawner.cs` — procedural ground-tile spawning
- `GroundTile.cs` — obstacle and coin spawning
- `Coin.cs` — collectible behaviour
- `GameManager.cs` — score and speed progression
- `CameraFollow.cs` — camera tracking

The repository also contains prefabs for ground tiles, obstacles and coins.

## Gameplay loop

```text
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
```

The ground spawner creates an initial sequence of tiles and then places obstacles and collectibles on subsequent tiles.

## Run locally

1. Clone the repository.
2. Open the project with Unity.
3. Open `Assets/Scenes/SampleScene.unity`.
4. Press **Play**.

Basic controls:

| Action | Key |
| --- | --- |
| Move horizontally | A / D or arrow keys |
| Jump | Space |

## Repository structure

```text
Assets/
├── Prefabs/
│   ├── Coin.prefab
│   ├── GroundTile.prefab
│   └── Obstacle.prefab
├── Scenes/
├── Scripts/
└── Materials/
```

## Project status

A compact gameplay prototype focused on movement, spawning, collectibles, scoring and restart flow.

## License

See [LICENSE](LICENSE).
