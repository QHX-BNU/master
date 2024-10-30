# Download
https://github.com/eladsegal/strategyqa/tree/main

# Paper
https://arxiv.org/abs/1811.00937

# Description
| Field         | Annotation                        | Example                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| qid           | the id of the question            | 2bc9c4f9c19c167187f2                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| term          | the term of the question          | Genghis Khan                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| description   | the description about the term    | founder and first Great Khan of the Mongol Empire                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| question      | the text of the question          | Are more people today related to Genghis Khan than Julius Caesar?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| answer        | the answer to the question        | true                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| facts         | the facts support the answer      | [<br>"Julius Caesar had three children.",<br> "Genghis Khan had sixteen children.",<br> "Modern geneticists have determined that  out of every 200 men today has DNA that can be traced to Genghis Khan."<br>        ]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| decomposition | the decomposition of the question | [<br>            "How many kids did Julius Caesar have?",<br>            "How many kids did Genghis Khan have?",<br>            "Is #2 greater than #1?"<br>        ]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| evidence      | the evidence of the question      |  [<br>            [<br>                [<br>                    [<br>                        "Caesarion-2",<br>                        "Julia (daughter of Caesar)-1"<br>                    ]<br>                ],<br>                [<br>                    [<br>                        "Alakhai Bekhi-1",<br>                        "Tolui-1"<br>                    ],<br>                    "no_evidence"<br>                ],<br>                [<br>                    "operation"<br>                ]<br>            ],<br>            [<br>                [<br>                    [<br>                        "Julius Caesar-75"<br>                    ]<br>                ],<br>                [<br>                    [<br>                        "Genghis Khan-17"<br>                    ]<br>                ],<br>                [<br>                    "operation"<br>                ]<br>            ],<br>            [<br>                [<br>                    [<br>                        "Gaius Julius Caesar-7"<br>                    ]<br>                ],<br>                [<br>                    [<br>                        "Genghis Khan-15"<br>                    ],<br>                    "no_evidence"<br>                ],<br>                [<br>                    "no_evidence",<br>                    "operation"<br>                ]<br>            ]<br>        ] |