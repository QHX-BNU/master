# Download
https://github.com/google-deepmind/AQuA

# Description
| Field     | Annotation                    | Example                                                                                                                                                                                                                           |
| --------- | ----------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| question  | the text of the question      | Two friends plan to walk along a 43-km trail, starting at opposite ends of the trail at the same time. If Friend P's rate is 15% faster than Friend Q's, how many kilometers will Friend P have walked when they pass each other? |
| options   | the options of the question   | ["A)21", "B)21.5", "C)22", "D)22.5", "E)23"]                                                                                                                                                                                      |
| rationale | the rationale of the question | If Q complete x kilometers, then P completes 1.15x kilometers.\nx + 1.15x = 43\n2.15x=43\nx = 43/2.15 = 20\nThen P will have have walked 1.15*20=23 km.\nThe answer is E.                                                         |
| answers   | the answer to the question    | E                                                                                                                                                                                                                                 |
