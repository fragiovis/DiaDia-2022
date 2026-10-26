# 🏫 DiaDia — Text Adventure at Roma Tre

*Object-Oriented Programming course (Programmazione Orientata agli Oggetti) · Università degli Studi Roma Tre (2023) · team homework*

A console text adventure set in the university building. You move between rooms, pick up and drop items and try to reach the winning room before you run out of energy (CFU).

## Commands
| Command | Effect |
|---|---|
| `vai <direzione>` | move to the adjacent room (`nord`, `sud`, `est`, `ovest`) |
| `prendi <attrezzo>` | pick up an item from the room |
| `posa <attrezzo>` | drop an item from your bag |
| `aiuto` | list the commands |
| `fine` | quit the game |

## Design
- `ambienti` — `Labirinto` (the map) and `Stanza` (a room with exits and items)
- `giocatore` — `Giocatore` (the player and their energy) and `Borsa` (a bag with a weight limit)
- `attrezzi` — `Attrezzo` (an item with name and weight)
- `Partita` (game state), `Comando` (command parsing) and `IOConsole` (input/output)
- **JUnit** tests for `Borsa`, `Giocatore`, `Partita` and `Stanza`

## Running it
```bash
javac -d out $(find src -name "*.java")
java -cp out it.uniroma3.diadia.DiaDia
```

## Tech stack
Java · JUnit
