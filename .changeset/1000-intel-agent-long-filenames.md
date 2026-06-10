---
type: Fixed
pr: 1003
---
**`gsd-intel-updater` now writes the canonical long intel filenames the `gsd-tools intel` CLI reads** — the agent prompt previously instructed short names (`files.json`, `apis.json`, `deps.json`, markdown `arch.md`) that the `INTEL_FILES` registry never reads, so `intel status`/`validate` reported the files missing and `intel query` returned nothing after `/gsd:map-codebase --query refresh`. `arch-decisions.json` is now emitted as queryable JSON. (#1000)
