# Download
https://huggingface.co/datasets/ChilleD/SVAMP?row=0

# Paper
https://aclanthology.org/2021.naacl-main.168.pdf

# Description
| Field           | Annotation                   | Example                                                                                                                                                                            |
| --------------- | ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id              | the id of the question       | chal-777                                                                                                                                                                           |
| body            | the context of the question  | There are 87 oranges and 290 bananas in Philip's collection. If the bananas are organized into 2 groups and oranges are organized into 93 groups                                   |
| question        | the text of the question     | How big is each group of bananas?                                                                                                                                                  |
| equation        | the equation of the question | ( 290.0 / 2.0 )                                                                                                                                                                    |
| answer          | the location of the mistake  | 145                                                                                                                                                                                |
| type            | the type of the question     | Common-Division                                                                                                                                                                    |
| question_concat | the body and the question    | There are 87 oranges and 290 bananas in Philip's collection. If the bananas are organized into 2 groups and oranges are organized into 93 groups How big is each group of bananas? |