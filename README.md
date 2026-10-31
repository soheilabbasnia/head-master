# HeadMaster — CLI Task Management

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-3776AB.svg?logo=python&logoColor=white)](https://python.org)
[![Database: SQLite3](https://img.shields.io/badge/Database-SQLite3-003B57.svg?logo=sqlite&logoColor=white)](https://sqlite.org)
[![Interface: CLI](https://img.shields.io/badge/Interface-CLI%20%2F%20Terminal-black.svg)](#)

English | [فارسی](README_FA.md)

A lightweight, persistent command-line **Task Management** console application built with **Python**, **SQLite3**, and **Colorama**.

---

## Overview

Staying organized from within the developer terminal boosts focus and productivity. **HeadMaster** provides an interactive command shell that manages your daily tasks, reminders, and todos directly from the console with persistent SQLite database storage.

Key highlights:
- **Persistent Local Database**: Built-in SQLite database engine storing tasks safely across sessions.
- **Interactive Console REPL**: Fast, responsive prompt supporting essential task management commands.
- **Visual Terminal Polish**: Enhanced with Colorama ANSI colors, status indicators, and animated terminal spinners.
- **Defensive Error Handling**: Automatic table generation, input bounds verification, and graceful exception handling.

---

## Features & Command Reference

| Command | Action | Description |
| :--- | :--- | :--- |
| `list` | View Tasks | Displays all pending and registered tasks formatted with their database IDs |
| `add` | Create Task | Prompts for task details and inserts a new record into the SQLite database |
| `edit` | Modify Task | Updates an existing task by its ID number |
| `remove` | Delete Task | Safely deletes a completed or unwanted task by ID |
| `cls` | Clear Screen | Clears the terminal screen for a distraction-free view |
| `restart` | Reload App | Reinitializes database connections and resets the console loop |
| `exit` | Terminate | Exits the application cleanly |

---

## Getting Started

### Prerequisites

- Python 3.7 or higher
- `colorama` library

### Installation & Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/soheilabbasnia/head-master.git
   cd head-master
   ```

2. **Install dependency**:
   ```bash
   pip install colorama
   ```

3. **Start HeadMaster**:
   ```bash
   python3 program.py
   ```

---

## Project Structure

```text
head-master/
├── database/
│   └── dB.py               # SQLite connection, schema creation & CRUD operations
├── style/
│   ├── color.py            # ANSI terminal color formatting helpers
│   └── loading.py          # Animated terminal spinner effects
├── actions.py              # Command dispatcher and interactive prompt handlers
├── program.py              # Application bootstrap and main interactive REPL
├── LICENSE                 # MIT License
└── README.md               # English project documentation
```

---

## Contributing

Contributions, feature requests, and CLI improvements are welcome!
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/due-dates`).
3. Commit your changes (`git commit -m 'Add due date and priority support'`).
4. Push to the branch (`git push origin feature/due-dates`).
5. Open a Pull Request.

---

## License

This project is licensed under the [MIT License](LICENSE).
Free and open-source for personal and educational use.

