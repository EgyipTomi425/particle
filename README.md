# particle

Particle simulation project.

## Structure

- `articles/` — articles and notes.
- `files/` — project files.
- `src/` — application source code (currently empty).
- `outputs/` — generated simulation outputs (ignored by Git, except for the `.gitkeep` placeholder).
- `submodules/geant4/` — Git submodule referencing [EgyipTomi425/geant4](https://github.com/EgyipTomi425/geant4) on its `master` branch.
- `submodules/Particle_Physics_Visualization/` — Git submodule referencing [martinsandor707/Particle_Physics_Visualization](https://github.com/martinsandor707/Particle_Physics_Visualization) on its `main` branch.

## Clone

```sh
git clone --recurse-submodules https://github.com/EgyipTomi425/particle.git
```

## Update submodules

```sh
git submodule update --remote
git add submodules/geant4 submodules/Particle_Physics_Visualization
git commit -m "Update submodules"
```

The `particle` repository uses `master`. Each submodule tracks its own configured branch.
