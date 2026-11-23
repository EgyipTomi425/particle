# particle

Particle simulation project.

## Structure

- `articles/` — articles and notes.
- `files/` — project files.
- `src/` — application source code (currently empty).
- `outputs/` — generated simulation outputs (ignored by Git, except for the `.gitkeep` placeholder).
- `submodules/geant4/` — Git submodule referencing [EgyipTomi425/geant4](https://github.com/EgyipTomi425/geant4) on its `master` branch.
- `submodules/Particle_Physics_Visualization/` — Git submodule referencing [martinsandor707/Particle_Physics_Visualization](https://github.com/martinsandor707/Particle_Physics_Visualization) on its `main` branch.
- `submodules/shape-form-particle/` — Git submodule referencing [EgyipTomi425/shape-form-particle](https://github.com/EgyipTomi425/shape-form-particle) on its `master` branch: analytic 3D shower-shape formulas (electron, muon, pion, proton) fitted to the LFHCal simulation.
- `submodules/models-particle/` — Git submodule referencing [EgyipTomi425/models-particle](https://github.com/EgyipTomi425/models-particle) on its `master` branch: calorimeter neural-network models (segmentation, incidence angle, momentum).
- `submodules/Echter_XGBoost/` — Git submodule referencing [EgyipTomi425/Echter_XGBoost](https://github.com/EgyipTomi425/Echter_XGBoost) on its `main` branch: GPU inference for XGBoost regression models in C++20 (CUDA, cuDF).

## Clone

```sh
git clone --recurse-submodules https://github.com/EgyipTomi425/particle.git
```

## Update submodules

```sh
git submodule update --remote
git add submodules/geant4 submodules/Particle_Physics_Visualization submodules/shape-form-particle submodules/models-particle submodules/Echter_XGBoost
git commit -m "Update submodules"
```

The `particle` repository uses `master`. Each submodule tracks its own configured branch.
