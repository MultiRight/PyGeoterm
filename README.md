# pygeoterm

A terminal-based geometric area calculator written in Python.

---

## Description

pygeoterm is a lightweight command-line tool that allows users to calculate the area of common geometric shapes directly from the terminal. It is designed to be simple, interactive, and accessible to anyone who needs quick geometric computations without relying on external tools or graphical interfaces.

---

## Features

- Calculate the area of seven geometric shapes:
  - Square
  - Rectangle
  - Triangle
  - Circle
  - Parallelogram
  - Trapezoid
  - Rhombus
- Color-coded terminal output for better readability
- Built-in error handling with descriptive error codes
- Interactive session with reset and exit options
- No external dependencies beyond the Python standard library

---

## Requirements

- Python 3.x

---

## Installation

Clone the repository:

```bash
git clone https://github.com/MultiRight/pygeoterm.git
cd pygeoterm
```

---

## Usage

Run the script with Python:

```bash
python pygeoterm.py
```

> **Tip:** If `python` does not work, try:
> ```bash
> python3 pygeoterm.py
> ```

Once launched, follow the on-screen prompts to select a geometric shape and enter the required dimensions. The program will output the calculated area.

To display the help information:

```bash
--help
```

At the end of each session, type `r` to restart or `q` to quit the program.

---

## Error Codes

| Code   | Description                                                        |
|--------|--------------------------------------------------------------------|
| err101 | Invalid input — letters or symbols were entered instead of numbers |
| err102 | Invalid shape — the selected choice is not in the geometric menu   |
| err103 | Invalid action — the input is neither `r` or `q`                   |

---

## License

This project is licensed under the **[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)** 

---


## 🐱 Special Thanks

A special thanks to mimi — the legendary, the great, the gentle cat.
