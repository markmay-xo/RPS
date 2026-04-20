# Rock Paper Scissors Scorer — Part 2

## Problem

Using the same scoring rules from Part 1, the second column no longer represents Player 2's choice — it represents the **outcome Player 2 needs to achieve**.

Given Player 1's choice and Player 2's required outcome, determine what Player 2 must have played, then score both players normally.

## New Meaning of Column 2

The letters now represent the required outcome for Player 2:

- `R` = Player 2 must **Lose**
- `P` = Player 2 must **Draw**
- `S` = Player 2 must **Win**

Player 1's column is unchanged — it still represents their choice (Rock, Paper, or Scissors).

## Example

**Input:**

```
R S
P R
S S
```

**Walkthrough:**

| Round | P1 Play  | P2 Outcome | P2 Must Play | Result  | P1 Round Score | P2 Round Score |
|-------|----------|------------|--------------|---------|----------------|----------------|
| 1     | Rock     | Win        | Paper        | P2 wins | 1 + 0 = 1     | 2 + 6 = 8     |
| 2     | Paper    | Lose       | Rock         | P1 wins | 2 + 6 = 8     | 1 + 0 = 1     |
| 3     | Scissors | Win        | Rock         | P2 wins | 3 + 0 = 3     | 1 + 6 = 7     |

**Output:**

```
Player 1: 12
Player 2: 16
```
