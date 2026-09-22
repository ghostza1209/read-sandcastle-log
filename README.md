# read-sandcastle-log

Renders a raw `.sandcastle/logs/*.log` file as a condensed, human-readable summary: a k9s-style header + run table, then per-run detail with tool calls laid out as an aligned table.

- In a real terminal: full-screen TUI, one tab per `*.log` file, live-follows the active tab like `tail -f`.
- Piped or redirected: prints the report for a single resolved file as plain text once.

## Install

```sh
git clone git@github.com:ghostza1209/read-sandcastle-log.git
ln -s "$PWD/read-sandcastle-log/read-sandcastle-log" ~/.local/bin/read-sandcastle-log
```

## Usage

```sh
read-sandcastle-log [path-to-log-or-dir]
```

Defaults to `.sandcastle/logs` in the current directory.
