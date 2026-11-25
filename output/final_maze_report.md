# Final Maze Exploration Report

## 1. Secret Message

> Welcome to the start of the course! Prepare for 3 intensive weeks ahead.

## 2. Autonomous Agent Results

| Metric | Result |
| :--- | ---: |
| Exit detected | True |
| Final model response received | True |
| Webpage calls | 10 |
| Room-page visits | 9 |
| Unique rooms visited | 9 |
| Total tokens used | 29,046 |
| Maximum allowed calls | 30 |

## 3. Actual Webpage Visit History

1 → 14 → 62 → 39 → 71 → 48 → 83 → 25 → 35

## 4. Physical Route Including Backtracking

1 → 14 → 62 → 39 → 71 → 39 → 62 → 48 → 83 → 25 → 35

## 5. Unique Rooms Visited

1, 14, 25, 35, 39, 48, 62, 71, 83

## 6. Dead End

Room 71 was a dead end. The agent identified the dead end and used the known connection back toward Room 39.

## 7. Unexplored Connections

- Room 27, discovered from Room 1.
- Room 56, discovered from Room 83.

## 8. Reflection

The agent successfully explored the maze using an autonomous tool-calling loop. The language model decided which room to explore next, while Python executed webpage requests and returned the results.

The agent handled a dead end and continued exploring until it found the exit and secret message.

One limitation is that the model maintained much of the maze map and backtracking information in its conversation rather than in a dedicated Python graph. A future improvement would be to store rooms, connections, and visited states in structured Python data.

## 9. Conclusion

The autonomous agent successfully found the maze exit, retrieved the secret message, and produced room-by-room exploration reports.
