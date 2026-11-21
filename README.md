# particle

Particle simulation project.

## Structure

- `articles/` — articles and notes.
- `files/` — project files.
- `src/` — application source code (currently empty).
- `outputs/` — generated simulation outputs (ignored by Git, except for the `.gitkeep` placeholder).
- `submodules/geant4/` — Git submodule referencing [EgyipTomi425/geant4](https://github.com/EgyipTomi425/geant4) on its `master` branch.

## Clone

```sh
git clone --recurse-submodules https://github.com/EgyipTomi425/particle.git
```

## Update Geant4 submodule

```sh
git submodule update --remote submodules/geant4
git add submodules/geant4
git commit -m "Update Geant4 submodule"
```
