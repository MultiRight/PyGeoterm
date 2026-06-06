# Changelog — PyGeoterm

All notable changes to this project are documented in this file.

---

## [v1.0.0] — Initial Release

Source: https://github.com/MultiRight/PyGeoterm/tree/c9f5d6f435c78837e2865d510de7db7453760c82

### Added
- Six geometric shapes: Square, Rectangle, Triangle, Circle, Parallelogram, Trapezoid
- Color-coded terminal output using ANSI escape codes
- Basic error handling via `try/except ValueError` with `err101`, `err102`, `err103`
- Help menu accessible via `--help`
- Session control with `reset` and `exit` commands

### Notes
- Color variables were defined inside the main loop
- No input retry logic — invalid input terminated the current session
- All error messages (`err101`, `err102`, `err103`) caused an abrupt exit instead of prompting the user again

---

## [v2.0.0] — Structural Improvement

Source: https://github.com/MultiRight/PyGeoterm/tree/0b4884e5112a6012902a5563ad8fb3c8da24a56f

### Changed
- Color variables moved outside the main loop as constants
- Help menu expanded with clearer descriptions for each error code
- Geometric menu redesigned as an ASCII table for better readability
- Comments added to separate sections of the code
- `pow()` replaced with direct arithmetic expressions
- Author link added to session footer

### Notes
- Core loop structure remained `while True` with `break` and `continue`
- No input retry logic introduced yet
- All error messages (`err101`, `err102`, `err103`) still caused an abrupt exit instead of prompting the user again

---

## [v3.0.0] — Final Release

Source: https://github.com/MultiRight/PyGeoterm

### Added
- Rhombus as a seventh geometric shape
- `color_pink` as a new color variable for shape selection prompt
- `running` flag variable to control the main loop instead of relying solely on `break`
- Input retry logic — invalid input now prompts the user again instead of terminating
- Session control replaced: `r` for restart, `q` for quit
- `running = True` restored on restart to ensure the main loop re-enters correctly

### Changed
- Main loop changed from `while True` to `while running`
- Inner shape loop changed to `while running` to exit cleanly after a successful calculation
- Each shape block now uses a dedicated `while True` loop with `break` on success
- `restart` and `exit` commands replaced with `r` and `q`

### Fixed
- All error messages (`err101`, `err102`, `err103`) previously caused an abrupt exit; all now prompt the user to try again without terminating the session

### Notes
- Project structure remains a single flat file without functions or classes
- Due to the deeply nested loop architecture, the project is considered feature-complete
- Further development is not planned; the codebase is not structured to accommodate significant new features without a full rewrite
- Maintenance patches may be issued if bugs are found

Repository: https://github.com/MultiRight/PyGeoterm

---

## Status

PyGeoterm has fulfilled its purpose as a terminal-based geometric area calculator.
The project will not receive new features. Maintenance only.

---

Copyright (C) 2026 MultiRight — https://github.com/MultiRight
