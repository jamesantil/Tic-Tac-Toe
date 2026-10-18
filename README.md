# Tic-Tac-Toe in C++

A two-player, click-to-play Tic-Tac-Toe game written in C++ with the **simplecpp** graphics library (turtleSim), built in my first semester at IIT Bombay.

## Features

- Graphical 3×3 board drawn with turtle-graphics primitives
- Players alternate as **Circle** and **Cross** by clicking on cells
- Win detection across all rows, columns and diagonals, plus tie detection
- Ignores invalid clicks and already-filled cells
- Board resets after each game; click **Quit** to exit

## How win detection works

Each player's moves are stored in a single integer, with one digit per cell. A move adds a fixed amount to that cell's digit, so a cell taken by a player reads `9`. A win is then just a check of whether all three digits of any line equal `9`. This keeps the whole board state in two numbers instead of a 2-D array.

## Run it

Requires [simplecpp](https://www.cse.iitb.ac.in/~ranade/simplecpp/).

```bash
s++ Tic-Tac-Toe.cpp
./a.out
```
