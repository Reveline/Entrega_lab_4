# TreeMap Lab (C)

## Project Overview
A C programming lab implementing an ordered map using a Binary Search Tree (BST). Students implement core TreeMap operations in `treemap.c`.

## Tech Stack
- Language: C (C99)
- Build: `gcc -g -Wall -Werror`
- Testing: Custom C harness in `test.c`
- Debug: `gdb` (installed via `replit.nix`)

## Project Structure
- `treemap.h` — Public API: types (`TreeMap`, `Pair`) and function declarations
- `treemap.c` — **Student implementation file** (DO NOT modify — student exercises)
- `test.c` — Full test suite (includes `treemap.c` directly)
- `main.c` — Example usage
- `test.sh` — Compile & run script; shows OK/FAILED counts and handles git push
- `replit.nix` — Installs `gdb`
- `images/` — Diagram assets for README

## Workflow
- **Run Tests**: `bash test.sh` (console output)
  - Compiles `test.c` → `a.out`, runs tests, shows results
  - On pass: offers to push progress to GitHub
  - On runtime error: runs `gdb` for backtrace

## Exercises in treemap.c
1. `createTreeMap` — allocate and initialize the map struct
2. `searchTreeMap` — BST search, update `current` pointer
3. `insertTreeMap` — BST insert, no duplicate keys
4. `minimum` — find leftmost node in a subtree
5. `removeNode` — delete node (3 cases: no child, one child, two children)
6. `firstTreeMap` / `nextTreeMap` — in-order traversal
7. `upperBound` — find pair with key >= given key
