# Tyr Game Data

This repository is a read-only snapshot of exported Tyr game data and assets.

It is intended to be consumed as a Git submodule or other pinned data dependency for Tyr-related tools, websites, apps, and similar integrations. It is not an application codebase, and it is not a collaboration repo.

## Repo Role

- Read-only snapshot repository
- Intended for submodule-style consumption
- Intended to be used as reference/dependency data for Tyr-related integrations
- Produced from Stoke-controlled export tooling
- Not intended for issues, pull requests, or general development discussion

If the dataset changes, the expected workflow is to regenerate and update the snapshot from the export pipeline, not to hand-edit files in this repository.

## Contents

The current exported layout is:

```text
generated/
  runtime.json
  asset-manifest.json

assets/
  images/
    vehicles/
    abilities/
    ammo/
    components/
    talents/
    icons/
    maps/
      lobby/
      minimap/
  models/
    vehicles/
      *.glb
      *-visual.glb
      *-armor.json
```

## Notes

- This repository is a snapshot, not a working area.
- Do not treat it as a general-purpose public dataset.
- Do not add site-owned code or unrelated assets here.
- If the data contract changes, update this README together with the exported layout.
- Snapshot revisions are intended to be tagged as `CL-<N>` so consumers can pin a specific exported changelist.

## Rights

See [LICENSE](./LICENSE). This repository is licensed as Stoke Games data/assets material, not as open-source code.
