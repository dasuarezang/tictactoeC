# tictactoeC

A two-player **Tic-Tac-Toe** game for the terminal, written in C.

I made it as a personal project after my first year of Telecommunications Engineering, to practise structs, pointers and 2D arrays outside of class.

## How to play

```
  TICTACTOE
  | A  B  C
------------
1 | O     X
2 |    O
3 | X
TURN: 6 (CROSS)
Introduce coordenadas (Ej: 2B):
```

- Circles (`O`) move first, then players take turns.
- Enter a move as a row number plus a column letter, for example `2B`. Lowercase letters also work.
- The game ends when a player completes a row, column or diagonal, or in a draw after 9 moves.

## Build and run

```bash
gcc tictactoe.c -o tictactoe
./tictactoe
```

The game clears the screen with `system("clear")`, so it is meant to run in a Linux or macOS terminal.

## Code overview

| Function | Purpose |
|---|---|
| `print_tictactoe` | Draws the board and whose turn it is |
| `play_tictactoe` | Reads and checks a move, then places the symbol |
| `comprove_conex` | Checks rows, columns and diagonals for a winner |

`TICTACTOE.txt` is a plain-text copy of the source code.
