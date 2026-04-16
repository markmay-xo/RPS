# Rock Paper Scissors Scorer

## Problem

Parse a series of Rock Paper Scissors rounds and calculate the total score for each player.

## Rules

Standard Rock Paper Scissors:

- Rock beats Scissors
- Scissors beats Paper
- Paper beats Rock

## Scoring

Each round, a player's score is the **sum** of their choice score and their outcome score.

**Choice scores:**

| Choice   | Score |
|----------|-------|
| Rock     | 1     |
| Paper    | 2     |
| Scissors | 3     |

**Outcome scores:**

| Outcome | Score |
|---------|-------|
| Lose    | 0     |
| Draw    | 3     |
| Win     | 6     |

**Examples:** Win with Rock = 1 + 6 = 7. Draw with Scissors = 3 + 3 = 6.

## Input

Each line contains two characters separated by a space representing Player 1's choice and Player 2's choice. Assume input is always valid.

- `R` = Rock
- `P` = Paper
- `S` = Scissors

```
<Player 1> <Player 2>
<Player 1> <Player 2>
...
```

## Output

Print the final total score for each player:

```
Player 1: <score>
Player 2: <score>
```

## Example

**Input:**

```
R P
P P
S P
```

**Walkthrough:**

| Round | P1 Play | P2 Play | Result  | P1 Round Score | P2 Round Score |
|-------|---------|---------|---------|----------------|----------------|
| 1     | Rock    | Paper   | P2 wins | 1 + 0 = 1     | 2 + 6 = 8     |
| 2     | Paper   | Paper   | Draw    | 2 + 3 = 5     | 2 + 3 = 5     |
| 3     | Scissors| Paper   | P1 wins | 3 + 6 = 9     | 2 + 0 = 2     |

**Output:**

```
Player 1: 15
Player 2: 15
```
