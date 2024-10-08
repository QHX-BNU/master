https://github.com/google-deepmind/AQuA/blob/master/README.md

# Description

| Field     | Annotation                                                        | Example                                                                                                                            |
| --------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| question  | A natural language definition of the problem to solve             | A grocery sells a bag of ice for $1.25, and makes 20% profit. If it sells 500 bags of ice, how much total profit does it make?<br> |
| options   | 5 possible options (A, B, C, D and E), among which one is correct | <br>"A)125", "B)150", "C)225", "D)250", "E)275"<br>                                                                                |
| rationale | A natural language description of the solution to the problem     | <br>Profit per bag = 1.25 * 0.20 = 0.25\nTotal profit = 500 * 0.25 = 125\nAnswer is A.                                             |
| correct   | The correct option                                                | A                                                                                                                                  |
