# freqtrade-strategies: portable verification records

Full raw logs are retained in the workspace maintenance evidence, not distributed here. Hashes identify those original logs. A successful build or selected test subset does not imply a full test-suite pass. Commands containing <workspace> describe the original execution environment.

[Machine-readable records](verification.json) · [Repository validation summary](../validation.md)

## Executed commands

| Check | Exit | Duration | Command | Outcomes |
| --- | ---: | ---: | --- | --- |
| build | 0 | 0.88s | `uv build --python 3.15` | Successfully built dist/freqtrade_strategies-0.1.0.tar.gz<br>Successfully built dist/freqtrade_strategies-0.1.0-py3-none-any.whl |
| compile | 0 | 0.13s | `<workspace>/freqtrade-strategies/.venv/bin/python -m compileall -q src` | See exit status; no test-count assertion. |
| final-build | 0 | 1.26s | `uv build --python 3.15.0` | Successfully built dist/freqtrade_strategies-0.1.0.tar.gz<br>Successfully built dist/freqtrade_strategies-0.1.0-py3-none-any.whl |
| final-build-2 | 0 | 0.95s | `uv build --python 3.15.0` | Successfully built dist/freqtrade_strategies-0.1.0.tar.gz<br>Successfully built dist/freqtrade_strategies-0.1.0-py3-none-any.whl |
| final-compile | 0 | 0.08s | `.venv/bin/python -m compileall -q src` | See exit status; no test-count assertion. |
| final-compile-2 | 0 | 0.08s | `.venv/bin/python -m compileall -q src` | See exit status; no test-count assertion. |
| final-lock | 0 | 0.2s | `uv lock --upgrade` | See exit status; no test-count assertion. |
| final-lock-2 | 0 | 0.18s | `uv lock --upgrade` | See exit status; no test-count assertion. |
| final-sync | 0 | 0.03s | `uv sync --all-extras --frozen --python 3.15.0` | See exit status; no test-count assertion. |
| final-sync-2 | 0 | 0.02s | `uv sync --all-extras --frozen --python 3.15.0` | See exit status; no test-count assertion. |
| lock-3.15 | 0 | 0.24s | `uv lock --upgrade --python 3.15` | See exit status; no test-count assertion. |
| sync-3.15 | 0 | 0.57s | `uv sync --all-extras --python 3.15` | See exit status; no test-count assertion. |
| tests | 5 | 0.56s | `<workspace>/freqtrade-strategies/.venv/bin/python -m pytest tests` | See exit status; no test-count assertion. |
