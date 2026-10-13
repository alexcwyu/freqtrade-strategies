# freqtrade-strategies maintenance validation

<!-- current-documentation-provenance -->
Documentation reviewed: 2026-10-13 / Git source base: `b5b33f2b2d793faa382d8c346db8a7bba9cca3b6` / [Current architecture and feature guide](ayu-develop.md).
Historical execution commands/results below retain their original dates and scope; this metadata update is not a new application test run.
<!-- /current-documentation-provenance -->


Recorded 2026-10-12T01:32:45.207790+08:00. Branch `feature/ayu_develop`; upstream default `upstream/main` is merged: **true**. Branch/tag synchronization records are retained in the workspace maintenance evidence. Feature branch publication is coordinated separately.

Runtime: **CPython 3.15.0**, uv **0.13.0**, build backend `hatchling.build`. Python 3.15.0 installs the archive environment. Strategy execution additionally requires a separately installed Freqtrade host.

Existing suite: **no tests ran in 0.01s** (exit `5`). The archive builds and all strategy source compiles. pytest exits 5 because this repository has no existing test cases; no cases were introduced.

No test cases were added. Existing assertions and strict warning behavior remain active; repaired fixtures own their loops, sessions, files and configuration paths. Existing upstream platform skips and configured deselections are reported exactly.

## Final build commands

| Check | Exact command | Exit | Seconds |
| --- | --- | ---: | ---: |
| lock | `uv lock --upgrade` | 0 | 0.18 |
| sync | `uv sync --all-extras --frozen --python 3.15.0` | 0 | 0.02 |
| build | `uv build --python 3.15.0` | 0 | 0.95 |
| compile | `.venv/bin/python -m compileall -q src` | 0 | 0.08 |

## Existing test and compatibility evidence

| Check | Exact command | Exit | Result |
| --- | --- | ---: | --- |
| lock-3.15 | `uv lock --upgrade --python 3.15` | 0 | Check completed; see exact exit code. |
| sync-3.15 | `uv sync --all-extras --python 3.15` | 0 | Check completed; see exact exit code. |
| tests | `/Users/alex/workspaces/trading/freqtrade-strategies/.venv/bin/python -m pytest tests` | 5 | no tests ran in 0.01s |

Raw logs remain in the workspace maintenance evidence directory. The [portable verification record](maintenance/verification.json) retains exact command arrays, exits, timing, runtime inventory and log filenames. Earlier failed attempts remain recorded and are not treated as successful final validation.

## Installed dependency versions

This is the selected environment after locked synchronization; isolated wheel build dependencies are resolved by the build backend and recorded in build output.

| Distribution | Version |
| --- | --- |
| freqtrade-strategies | 0.1.0 |
| iniconfig | 2.3.1 |
| nodeenv | 1.11.0 |
| packaging | 26.3 |
| pluggy | 1.6.0 |
| Pygments | 2.21.0 |
| pyright | 1.1.414 |
| pytest | 9.1.1 |
| ruff | 0.17.0 |
| typing_extensions | 4.16.0 |

See [architecture](ayu-develop.md) for source-linked component/sequence/workflow diagrams and [development](development.md) for reproducible uv commands.
