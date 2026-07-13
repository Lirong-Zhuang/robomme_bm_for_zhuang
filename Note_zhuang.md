## Virtual Environments

Activate:

```bash
source .venv/bin/activate
```

Deactivate:

```bash
deactivate
```


## Run a reproduction of oracle as subgoals predictor

Change scripts/dataset_replay.py line 256-258 to change the setup

```bash
uv run scripts/dataset_replay.py
```

Replay one episode or several selected episodes with `--episode-indices`:

```bash
uv run scripts/dataset_replay.py --task-id BinFill --episode-indices 7
uv run scripts/dataset_replay.py --task-id BinFill --episode-indices 3 7 12
```

When `--episode-indices` is set, it takes precedence over `--replay-number`.
