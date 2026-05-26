# DrRacket Config

[English](README.md) | [中文](README.zh-CN.md)

Modern keybindings for DrRacket with REPL integration. Provides Emacs-style incremental evaluation — send expressions and selections directly to the REPL without leaving the editor.

## Features

- **Send to REPL** — Evaluate expressions incrementally, Emacs-style
  - Send the current top-level expression
  - Send the selected region
  - Optionally shift focus to the REPL panel after sending

## Requirements

- DrRacket 7.0 or later

## Installation

1. Clone this repository:

```bash
git clone https://github.com/jrtxio/drracket-config.git
```

2. In DrRacket:
   - Go to **Edit** → **Keybindings** → **Add User-defined Keybindings...**
   - Select `drracket-keybindings.rkt` from the cloned directory
   - Restart DrRacket

## Keybindings

| Shortcut | Action |
|----------|--------|
| `Ctrl+C, Ctrl+E` | Send current expression to REPL |
| `Ctrl+C, Ctrl+R` | Send selected code to REPL |
| `Ctrl+C, Alt+E` | Send expression and focus REPL |
| `Ctrl+C, Alt+R` | Send selection and focus REPL |

**Usage:**

- Place cursor in or near an expression
- Press `Ctrl+C` then `Ctrl+E` to evaluate it in the REPL
- Or select code and press `Ctrl+C` then `Ctrl+R`

**Note:** You must run the program at least once (F5) to initialize the REPL before using these keybindings.

## Tips

- **View all active keybindings:** Edit → Keybindings → Show Active Keybindings

## Updating

```bash
cd /path/to/drracket-config
git pull
```

Then restart DrRacket.

## License

[MIT](LICENSE)
