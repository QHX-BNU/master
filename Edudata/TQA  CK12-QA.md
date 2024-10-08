https://github.com/dreamrealise/QA-Survey/blob/master/%E8%A1%A8%E6%A0%BC%E9%97%AE%E7%AD%94(Table_Question_Answering%2CTQA)-%E5%AD%A6%E6%9C%AF%E7%95%8C.md
数据集：
https://www.kaggle.com/datasets/gopalmahadevan/textbook-question-answering-tqa-dataset/data
# Description

| Field                 | Annotation                                                            | Example                        |
| --------------------- | --------------------------------------------------------------------- | ------------------------------ |
| questions             | questions that should be answerable given the contents of the lesson. | [[TQA  CK12-QA#tip1]]          |
| topics                | the topics of the questions                                           | [[TQA  CK12-QA#tip2]]          |
| adjunctTopics         | the adjunctTopics of the questions                                    | [[TQA  CK12-QA#tip3]]          |
| diagramAnnotations    | the diagram Annotations of the questions                              | [[TQA  CK12-QA#tip4]]          |
| instructionalDiagrams | the instructional Diagrams of the questions                           | [[TQA  CK12-QA#tip5]]          |
| LessonName            | the name of the lesson                                                | earth science and its branches |
| globalID              | the id of the question                                                | L_0002                         |

## tip1
- questions: questions that should be answerable given the contents of the lesson.
    
    - nonDiagramQuestions: questions with no accompanying diagram needed to answer
    - diagramQuestions: questions with an accompanying diagram needed to answer
        - questionType: format of the question, multiple choice, fill-in-the-blank, true/false, diagram multiple choice
        - beingAsked: text of the question being posed
        - idStructural: the original number or letter identifier in the source, e.g. "1.", "2.", "A."
        - globalID: dataset-unique id number assigned to the question
        - answerChoices: possible answer options- the number and form will depend on the question type
        - correctAnswer: the correct answer given for the question
        - imagePath: relative path to image file from the dataset root directory.
    {
  "diagramQuestions": {},
  "nonDiagramQuestions": {
    "NDQ_000046": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "solid Earth.",
          "rawText": "a. solid Earth."
        },
        "b": {
          "idStructural": "b.",
          "processedText": "Earths oceans.",
          "rawText": "b. Earths oceans."
        },
        "c": {
          "idStructural": "c.",
          "processedText": "Earths atmosphere.",
          "rawText": "c. Earths atmosphere."
        },
        "d": {
          "idStructural": "d.",
          "processedText": "all of the above",
          "rawText": "d. all of the above"
        }
      },
      "beingAsked": {
        "processedText": "Earth science is the study of",
        "rawText": "1. Earth science is the study of"
      },
      "correctAnswer": {
        "processedText": "d",
        "rawText": "1. d"
      },
      "globalID": "NDQ_000046",
      "idStructural": "1. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000047": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "mountains form.",
          "rawText": "a. mountains form."
        },
        "b": {
          "idStructural": "b.",
          "processedText": "people cause pollution.",
          "rawText": "b. people cause pollution."
        },
        "c": {
          "idStructural": "c.",
          "processedText": "tornadoes occur.",
          "rawText": "c. tornadoes occur."
        },
        "d": {
          "idStructural": "d.",
          "processedText": "two of the above",
          "rawText": "d. two of the above"
        }
      },
      "beingAsked": {
        "processedText": "A geologist would be most likely to investigate how",
        "rawText": "2. A geologist would be most likely to investigate how"
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "2. a"
      },
      "globalID": "NDQ_000047",
      "idStructural": "2. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000048": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "meteorologist",
          "rawText": "a. meteorologist"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "climatologist",
          "rawText": "b. climatologist"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geologist",
          "rawText": "c. geologist"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "ecologist",
          "rawText": "d. ecologist"
        }
      },
      "beingAsked": {
        "processedText": "Which type of Earth scientist might look for petroleum for an oil company?",
        "rawText": "3. Which type of Earth scientist might look for petroleum for an oil company?"
      },
      "correctAnswer": {
        "processedText": "c",
        "rawText": "3. c"
      },
      "globalID": "NDQ_000048",
      "idStructural": "3. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000049": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "human pollution of ocean water.",
          "rawText": "a. human pollution of ocean water."
        },
        "b": {
          "idStructural": "b.",
          "processedText": "naturally occurring elements in ocean water.",
          "rawText": "b. naturally occurring elements in ocean water."
        },
        "c": {
          "idStructural": "c.",
          "processedText": "rising levels of ocean water.",
          "rawText": "c. rising levels of ocean water."
        },
        "d": {
          "idStructural": "d.",
          "processedText": "rocks on the ocean floor.",
          "rawText": "d. rocks on the ocean floor."
        }
      },
      "beingAsked": {
        "processedText": "Chemical oceanography is the study of the",
        "rawText": "4. Chemical oceanography is the study of the"
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "4. b"
      },
      "globalID": "NDQ_000049",
      "idStructural": "4. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000050": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "planetary geologist.",
          "rawText": "a. planetary geologist."
        },
        "b": {
          "idStructural": "b.",
          "processedText": "seismologist.",
          "rawText": "b. seismologist."
        },
        "c": {
          "idStructural": "c.",
          "processedText": "physical oceanographer.",
          "rawText": "c. physical oceanographer."
        },
        "d": {
          "idStructural": "d.",
          "processedText": "climatologist.",
          "rawText": "d. climatologist."
        }
      },
      "beingAsked": {
        "processedText": "The problem of global warming is most likely to be the focus of a scientist known as a",
        "rawText": "5. The problem of global warming is most likely to be the focus of a scientist known as a"
      },
      "correctAnswer": {
        "processedText": "d",
        "rawText": "5. d"
      },
      "globalID": "NDQ_000050",
      "idStructural": "5. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000051": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "volcanologist",
          "rawText": "a. volcanologist"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "meteorologist",
          "rawText": "b. meteorologist"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "climatologist",
          "rawText": "c. climatologist"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental scientist",
          "rawText": "d. environmental scientist"
        }
      },
      "beingAsked": {
        "processedText": "Which type of Earth scientist would you expect to give a weather report?",
        "rawText": "6. Which type of Earth scientist would you expect to give a weather report?"
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "6. b"
      },
      "globalID": "NDQ_000051",
      "idStructural": "6. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000052": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "satellites.",
          "rawText": "a. satellites."
        },
        "b": {
          "idStructural": "b.",
          "processedText": "radar.",
          "rawText": "b. radar."
        },
        "c": {
          "idStructural": "c.",
          "processedText": "telescopes.",
          "rawText": "c. telescopes."
        },
        "d": {
          "idStructural": "d.",
          "processedText": "two of the above",
          "rawText": "d. two of the above"
        }
      },
      "beingAsked": {
        "processedText": "Tools typically used by meteorologists include",
        "rawText": "7. Tools typically used by meteorologists include"
      },
      "correctAnswer": {
        "processedText": "d",
        "rawText": "7. d"
      },
      "globalID": "NDQ_000052",
      "idStructural": "7. ",
      "questionSubType": "Multiple Choice",
      "questionType": "Multiple Choice"
    },
    "NDQ_000053": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of Earths weather",
        "rawText": "1. study of Earths weather"
      },
      "correctAnswer": {
        "processedText": "g",
        "rawText": "1.g"
      },
      "globalID": "NDQ_000053",
      "idStructural": "1.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000054": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of earthquakes",
        "rawText": "2. study of earthquakes"
      },
      "correctAnswer": {
        "processedText": "f",
        "rawText": "2.f"
      },
      "globalID": "NDQ_000054",
      "idStructural": "2.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000055": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of Earths oceans",
        "rawText": "3. study of Earths oceans"
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "3.b"
      },
      "globalID": "NDQ_000055",
      "idStructural": "3.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000056": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of solid Earth",
        "rawText": "4. study of solid Earth"
      },
      "correctAnswer": {
        "processedText": "c",
        "rawText": "4.c"
      },
      "globalID": "NDQ_000056",
      "idStructural": "4.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000057": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of human effects on Earth",
        "rawText": "5. study of human effects on Earth"
      },
      "correctAnswer": {
        "processedText": "d",
        "rawText": "5.d"
      },
      "globalID": "NDQ_000057",
      "idStructural": "5.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000058": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of all aspects of planet Earth",
        "rawText": "6. study of all aspects of planet Earth"
      },
      "correctAnswer": {
        "processedText": "e",
        "rawText": "6.e"
      },
      "globalID": "NDQ_000058",
      "idStructural": "6.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000059": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "astronomy",
          "rawText": "a. astronomy"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "oceanography",
          "rawText": "b. oceanography"
        },
        "c": {
          "idStructural": "c.",
          "processedText": "geology",
          "rawText": "c. geology"
        },
        "d": {
          "idStructural": "d.",
          "processedText": "environmental science",
          "rawText": "d. environmental science"
        },
        "e": {
          "idStructural": "e.",
          "processedText": "Earth science",
          "rawText": "e. Earth science"
        },
        "f": {
          "idStructural": "f.",
          "processedText": "seismology",
          "rawText": "f. seismology"
        },
        "g": {
          "idStructural": "g.",
          "processedText": "meteorology",
          "rawText": "g. meteorology"
        }
      },
      "beingAsked": {
        "processedText": "study of the universe",
        "rawText": "7. study of the universe"
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "7.a"
      },
      "globalID": "NDQ_000059",
      "idStructural": "7.",
      "questionSubType": "Matching",
      "questionType": "Multiple Choice"
    },
    "NDQ_000060": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Earth science is a branch of geology.",
        "rawText": "1. Earth science is a branch of geology."
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "1.false"
      },
      "globalID": "NDQ_000060",
      "idStructural": "1.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000061": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Some geologists specialize in the study of soil.",
        "rawText": "2. Some geologists specialize in the study of soil."
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "2.true"
      },
      "globalID": "NDQ_000061",
      "idStructural": "2.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000062": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Rock layers below Earths surface are a record of Earths history.",
        "rawText": "3. Rock layers below Earths surface are a record of Earths history."
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "3.true"
      },
      "globalID": "NDQ_000062",
      "idStructural": "3.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000063": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "The science of oceanography started with mapping the oceans.",
        "rawText": "4. The science of oceanography started with mapping the oceans."
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "4.true"
      },
      "globalID": "NDQ_000063",
      "idStructural": "4.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000064": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Scientists have not yet visited the deepest parts of the ocean.",
        "rawText": "5. Scientists have not yet visited the deepest parts of the ocean."
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "5.false"
      },
      "globalID": "NDQ_000064",
      "idStructural": "5.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000065": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Most of Earths water is in rivers and lakes.",
        "rawText": "6. Most of Earths water is in rivers and lakes."
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "6.false"
      },
      "globalID": "NDQ_000065",
      "idStructural": "6.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000066": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Humans have had relatively little impact on the oceans.",
        "rawText": "7. Humans have had relatively little impact on the oceans."
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "7.false"
      },
      "globalID": "NDQ_000066",
      "idStructural": "7.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000067": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "There are several branches of oceanography.",
        "rawText": "8. There are several branches of oceanography."
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "8.true"
      },
      "globalID": "NDQ_000067",
      "idStructural": "8.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000068": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "Meteorologists study meteors.",
        "rawText": "9. Meteorologists study meteors."
      },
      "correctAnswer": {
        "processedText": "b",
        "rawText": "9.false"
      },
      "globalID": "NDQ_000068",
      "idStructural": "9.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    },
    "NDQ_000069": {
      "answerChoices": {
        "a": {
          "idStructural": "a.",
          "processedText": "true",
          "rawText": "a. true"
        },
        "b": {
          "idStructural": "b.",
          "processedText": "false",
          "rawText": "b. false"
        }
      },
      "beingAsked": {
        "processedText": "The burning of fossil fuels contributes to global warming.",
        "rawText": "10. The burning of fossil fuels contributes to global warming."
      },
      "correctAnswer": {
        "processedText": "a",
        "rawText": "10.true"
      },
      "globalID": "NDQ_000069",
      "idStructural": "10.",
      "questionSubType": "True or False",
      "questionType": "Multiple Choice"
    }
  }
}
## tip2
- topic name: name string, e.g. Carboniferous Period, Cenozoic Era, Cretaceous Period
- content: instructional content extracted from source material
    - globalID: dataset-unique id number assigned to the topic
    - text: paragraph sized text blurb introducing and explaining topic
    - figures: diagram images associated with topic, if any
    - caption: image caption
    - imagePath: relative path to image file from the dataset root directory.
    - orderID: order of appearance within lesson
{
  "T_0016": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.11 (A) Mineralogists focus on all kinds of minerals. (B) Seismographs are used to measure earthquakes and pinpoint their origins.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20011.png"
        }
      ],
      "mediaLinks": [],
      "text": "Geology is the study of the solid Earth. Geologists study how rocks and minerals form. The way mountains rise up is part of geology. The way mountains erode away is another part. Geologists also study fossils and Earths history. There are many other branches of geology. There is so much to know about our home planet that most geologists become specialists in one area. For example, a mineralogist studies minerals, as seen in (Figure 1.11). Some volcanologists brave molten lava to study volcanoes. Seismologists monitor earthquakes worldwide to help protect people and property from harm (Figure 1.11). Paleontologists are interested in fossils and how ancient organisms lived. Scientists who compare the geology of other planets to Earth are planetary geologists. Some geologists study the Moon. Others look for petroleum. Still others specialize in studying soil. Some geologists can tell how old rocks are and determine how different rock layers formed. There is probably an expert in almost anything you can think of related to Earth! Geologists might study rivers and lakes, the underground water found between soil and rock particles, or even water that is frozen in glaciers. Earth scientists also need geographers who explore the features of Earths surface and work with cartographers, who make maps. Studying the layers of rock beneath the surface helps us to understand the history of planet Earth (Figure 1.12). "
    },
    "globalID": "T_0016",
    "topicName": "Geology"
  },
  "T_0017": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.12 These folded rock layers have bent over time. Studying rock layers helps scientists to explain these layers and the geologic history of the area.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20012.png"
        },
        {
          "caption": "FIGURE 1.13 This research vessel is specially designed to explore the seas around Antarctica.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20013.png"
        }
      ],
      "mediaLinks": [],
      "text": "Oceanography is the study of the oceans. The word oceanology might be more accurate, since ology is the study of. Graph is to write and refers to map making. But mapping the oceans is how oceanography started. More than 70% of Earths surface is covered with water. Almost all of that water is in the oceans. Scientists have visited the deepest parts of the ocean in submarines. Remote vehicles go where humans cant. Yet much of the ocean remains unexplored. Some people call the ocean the last frontier. Humans have had a big impact on the oceans. Populations of fish and other marine species have been overfished. Contaminants are polluting the waters. Global warming is melting the thick ice caps and warming the water. Warmer water expands and, along with water from the melting ice caps, causes sea levels to rise. There are many branches of oceanography. Physical oceanography is the study of water movement, like waves and ocean currents (Figure 1.13). Marine geology looks at rocks and structures in the ocean basins. Chemical oceanography studies the natural elements in ocean water. Marine biology looks at marine life. "
    },
    "globalID": "T_0017",
    "topicName": "Oceanography"
  },
  "T_0018": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.14 Meteorologists can help us to prepare for major storms or know if today is a good day for a picnic.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20014.png"
        },
        {
          "caption": "FIGURE 1.15 Carbon dioxide released into the atmo- sphere is causing global warming.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20015.png"
        }
      ],
      "mediaLinks": [],
      "text": "Meteorologists dont study meteors they study the atmosphere! The word meteor refers to things in the air. Meteorology includes the study of weather patterns, clouds, hurricanes, and tornadoes. Meteorology is very important. Using radars and satellites, meteorologists work to predict, or forecast, the weather (Figure 1.14). The atmosphere is a thin layer of gas that surrounds Earth. Climatologists study the atmosphere. These scientists work to understand the climate as it is now. They also study how climate will change in response to global warming. The atmosphere contains small amounts of carbon dioxide. Climatologists have found that humans are putting a lot of extra carbon dioxide into the atmosphere. This is mostly from burning fossil fuels. The extra carbon dioxide traps heat from the Sun. Trapped heat causes the atmosphere to heat up. We call this global warming (Figure 1.15). "
    },
    "globalID": "T_0018",
    "topicName": "Climatology and Meteorology"
  },
  "T_0019": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.16 In a marine ecosystem, coral, fish, and other sea life depend on each other for survival.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20016.png"
        }
      ],
      "mediaLinks": [],
      "text": "Environmental scientists study the ways that humans affect the planet we live on. We hope to find better ways of living that can also help the environment. Ecologists study lifeforms and the environments they live in (Figure 1.16). They try to predict the chain reactions that could occur when one part of the ecosystem is disrupted. "
    },
    "globalID": "T_0019",
    "topicName": "Environmental Science"
  },
  "T_0020": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "Astronomy and astronomers have shown that the planets in our solar system are not the only planets in the universe. Over 530 planets were known outside our solar system in 2011. And there are billions of other planets! The universe also contains black holes, other galaxies, asteroids, comets, and nebula. As big as Earth seems, the entire universe is vastly more enormous. Earth is just a tiny part of our universe. Astronomers use many tools to study things in space. Earth-orbiting telescopes view stars and galaxies from the darkness of space (Figure 1.17). They may have optical and radio telescopes to see things that the human eye cant see. Spacecraft travel great distances to send back information on faraway places. Astronomers ask a wide variety of questions. How do strong bursts of energy from the Sun, called solar flares, affect communications? How might an impact from an asteroid affect life on Earth? What are the properties of black holes? Astronomers ask bigger questions too. How was the universe created? Is there life on other planets? Are there resources on other planets that people could use? Astronomers use what Earth scientists know to make comparisons with other planets. "
    },
    "globalID": "T_0020",
    "topicName": "Astronomy"
  }
}
## tip3
- adjunctTopics:
    
    - section type: vocabulary, summary, introduction, apply concepts, etc.
    - content: instructional content extracted from source material
    - text: paragraph sized text blurb introducing and explaining topic
    - figures: diagram images associated with topic, if any
        - caption: image caption
        - imagePath: relative path to image file from the dataset root directory.
        - orderID: order of appearance within lesson
    {
  "Apply Concepts": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "5. A glacier is melting. What are all of the scientists you can think of who might be involved in studying this glacier? What would each of them do? "
    },
    "orderID": "t_12"
  },
  "Introduction": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.10 Earth as seen from Apollo 17.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20010.png"
        }
      ],
      "mediaLinks": [],
      "text": "Earth Science is the study of all aspects of our planet Earth. Earth Science is not just about the molten lava, icy mountain peaks, steep canyons and towering waterfalls of the continents. Earth Science includes the atmosphere and oceans. The field also looks out into the solar system, galaxy, and universe. Earth scientists seek to understand the beautiful planet on which we depend (Figure 1.10). Different branches of Earth Science study one particular part of Earth. Since all of the branches are connected, specialists work together to answer complicated questions. Lets look at some important branches of Earth Science. "
    },
    "orderID": "t_03"
  },
  "Lesson Objectives": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "Describe Earth Science and its branches.\nIdentify the field of geology as a branch of Earth Science that deals with the rocks and minerals of Earth.\nDescribe the field of oceanography as a branch of Earth Science that explores the ocean.\nDefine the field of meteorology as a branch of Earth Science that deals with the atmosphere.\nUnderstand that astronomy is a branch of Earth Science that studies our solar system and universe.\nList some of the other branches of Earth Science, and how they relate to the study of Earth.\n"
    },
    "orderID": "t_01"
  },
  "Lesson Summary": {
    "content": {
      "figures": [
        {
          "caption": "FIGURE 1.17 Scientists are using telescopes to search for other planets that may have conditions favorable for life. The places they can look are near our solar system in our galaxy.",
          "imagePath": "textbook_images/earth_science_and_its_branches_20017.png"
        }
      ],
      "mediaLinks": [],
      "text": "Earth science includes many fields of science related to our home planet. Geology is the study of Earths material and structures and the processes that create them. Oceanography is the study of the oceans: water movement, chemistry and the ocean basins among other things. Meteorologists study the atmosphere including climate and weather. Environmental science deals with the effects people have on the environment. Astronomers study Earths larger environment: the solar system, galaxy, and universe that our planet resides in. "
    },
    "orderID": "t_09"
  },
  "Points to Consider": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "Why is Earth Science so important? Which branch of Earth Science would you most like to explore? What is the biggest problem that we face today? Which Earth scientists may help us to solve the problem? What other branches of science or society are related to and necessary for Earth Science? "
    },
    "orderID": "t_14"
  },
  "Recall": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "1. What are three major branches of Earth Science? 2. What branch of science deals with stars and galaxies beyond Earth? 3. List important functions of Earth scientists. 4. What does a meteorologist study? "
    },
    "orderID": "t_11"
  },
  "Think Critically": {
    "content": {
      "figures": [],
      "mediaLinks": [],
      "text": "6. Design an experiment that you could conduct in any branch of Earth Science. Identify the independent variable and dependent variable. "
    },
    "orderID": "t_13"
  },
  "Vocabulary": {
    "astronomy": "",
    "geology": "the study of the rocks, processes, and history of Earth ",
    "meteorology": "",
    "oceanography": ""
  }
}
## tip4
- diagramAnnotations
    
    - diagram name: name of diagram image file (matching imageName field in diagramQuestions and instructionalDiagrams)
        - A list of groundtruth diagram text boxes with
            - text: human transcribed text
            - rectangle: location of text bounding box on the image in the form:  
                [lower left coordinate, upper right coordinate]
{
  "erosion_6843.png": [
    {
      "rectangle": [
        [
          729,
          210
        ],
        [
          887,
          278
        ]
      ],
      "text": "direction of cliff retreat"
    },
    {
      "rectangle": [
        [
          2,
          9
        ],
        [
          205,
          103
        ]
      ],
      "text": "1. large crack, opened up by hydraulic action"
    },
    {
      "rectangle": [
        [
          77,
          435
        ],
        [
          322,
          568
        ]
      ],
      "text": "2. the crack grows into a cave by hydraulic action and abrasion"
    },
    {
      "rectangle": [
        [
          472,
          198
        ],
        [
          604,
          227
        ]
      ],
      "text": "headland"
    },
    {
      "rectangle": [
        [
          678,
          440
        ],
        [
          880,
          507
        ]
      ],
      "text": "6. this leaves a tall rock stack"
    },
    {
      "rectangle": [
        [
          359,
          440
        ],
        [
          641,
          539
        ]
      ],
      "text": "4. the cave breaks through the headland forming a natural arch"
    },
    {
      "rectangle": [
        [
          301,
          9
        ],
        [
          451,
          111
        ]
      ],
      "text": "3. the cave becomes larger"
    },
    {
      "rectangle": [
        [
          804,
          9
        ],
        [
          963,
          140
        ]
      ],
      "text": "7. the stack is eroded forming"
    },
    {
      "rectangle": [
        [
          558,
          4
        ],
        [
          732,
          103
        ]
      ],
      "text": "5. the arch is eroded and collapses"
    }
  ],
  "erosion_6845.png": [
    {
      "rectangle": [
        [
          630,
          2
        ],
        [
          1018,
          32
        ]
      ],
      "text": "active beach system"
    },
    {
      "rectangle": [
        [
          812,
          97
        ],
        [
          952,
          138
        ]
      ],
      "text": "shoreface"
    },
    {
      "rectangle": [
        [
          1280,
          90
        ],
        [
          1442,
          155
        ]
      ],
      "text": "continental shelf"
    },
    {
      "rectangle": [
        [
          513,
          38
        ],
        [
          647,
          100
        ]
      ],
      "text": "intertidal beach"
    },
    {
      "rectangle": [
        [
          443,
          97
        ],
        [
          530,
          155
        ]
      ],
      "text": "upper beach"
    },
    {
      "rectangle": [
        [
          288,
          122
        ],
        [
          382,
          162
        ]
      ],
      "text": "dunes"
    },
    {
      "rectangle": [
        [
          67,
          473
        ],
        [
          257,
          557
        ]
      ],
      "text": "layered sedimentary rocks"
    },
    {
      "rectangle": [
        [
          335,
          528
        ],
        [
          468,
          590
        ]
      ],
      "text": "modern sediment"
    },
    {
      "rectangle": [
        [
          2,
          597
        ],
        [
          383,
          678
        ]
      ],
      "text": "fair-weather beach, sediment-limited"
    },
    {
      "rectangle": [
        [
          510,
          605
        ],
        [
          748,
          672
        ]
      ],
      "text": "rocks exposed on shoreface"
    },
    {
      "rectangle": [
        [
          1070,
          520
        ],
        [
          1228,
          587
        ]
      ],
      "text": "hardbottom (rock)"
    },
    {
      "rectangle": [
        [
          457,
          713
        ],
        [
          585,
          782
        ]
      ],
      "text": "intertidal beach"
    },
    {
      "rectangle": [
        [
          650,
          918
        ],
        [
          897,
          958
        ]
      ],
      "text": "fair-weather profile"
    },
    {
      "rectangle": [
        [
          18,
          1065
        ],
        [
          140,
          1123
        ]
      ],
      "text": "erosional scarp"
    },
    {
      "rectangle": [
        [
          140,
          1123
        ],
        [
          342,
          1178
        ]
      ],
      "text": "rocks exposed on beach"
    },
    {
      "rectangle": [
        [
          365,
          1228
        ],
        [
          610,
          1290
        ]
      ],
      "text": "sediment stored on lower shoreface"
    },
    {
      "rectangle": [
        [
          328,
          1343
        ],
        [
          -5,
          1262
        ]
      ],
      "text": "storm beach, sediment-limited"
    }
  ],
  "erosion_6846.png": [
    {
      "rectangle": [
        [
          413,
          248
        ],
        [
          561,
          263
        ]
      ],
      "text": "5. wave-cut platform"
    },
    {
      "rectangle": [
        [
          142,
          4
        ],
        [
          252,
          25
        ]
      ],
      "text": "4. cliff retreats"
    },
    {
      "rectangle": [
        [
          382,
          3
        ],
        [
          491,
          43
        ]
      ],
      "text": "1. original position of cliff"
    },
    {
      "rectangle": [
        [
          267,
          146
        ],
        [
          402,
          183
        ]
      ],
      "text": "3. notch increases and cliff collapses"
    },
    {
      "rectangle": [
        [
          349,
          209
        ],
        [
          476,
          228
        ]
      ],
      "text": "2. wave-cut notch"
    }
  ],
  "erosion_6850.png": [
    {
      "rectangle": [
        [
          361,
          178
        ],
        [
          437,
          222
        ]
      ],
      "text": "pebbles, stones and boulders"
    },
    {
      "rectangle": [
        [
          102,
          116
        ],
        [
          37,
          105
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          38,
          189
        ],
        [
          97,
          205
        ]
      ],
      "text": "soft rock"
    },
    {
      "rectangle": [
        [
          207,
          66
        ],
        [
          289,
          93
        ]
      ],
      "text": "hard rock topples over"
    },
    {
      "rectangle": [
        [
          33,
          21
        ],
        [
          150,
          40
        ]
      ],
      "text": "waterfall retreats"
    },
    {
      "rectangle": [
        [
          268,
          184
        ],
        [
          319,
          212
        ]
      ],
      "text": "plunge pool"
    },
    {
      "rectangle": [
        [
          446,
          280
        ],
        [
          545,
          297
        ]
      ],
      "text": "buzzle.com"
    },
    {
      "rectangle": [
        [
          361,
          125
        ],
        [
          495,
          141
        ]
      ],
      "text": "overhang collapses"
    },
    {
      "rectangle": [
        [
          35,
          241
        ],
        [
          162,
          261
        ]
      ],
      "text": "steep-sided gorge"
    },
    {
      "rectangle": [
        [
          92,
          87
        ],
        [
          57,
          75
        ]
      ],
      "text": "river"
    }
  ],
  "erosion_6851.png": [
    {
      "rectangle": [
        [
          488,
          17
        ],
        [
          612,
          61
        ]
      ],
      "text": "1. original shape of headland"
    },
    {
      "rectangle": [
        [
          157,
          138
        ],
        [
          234,
          168
        ]
      ],
      "text": "blowhole"
    },
    {
      "rectangle": [
        [
          293,
          132
        ],
        [
          373,
          158
        ]
      ],
      "text": "headland"
    },
    {
      "rectangle": [
        [
          455,
          138
        ],
        [
          504,
          162
        ]
      ],
      "text": "stack"
    },
    {
      "rectangle": [
        [
          310,
          190
        ],
        [
          358,
          215
        ]
      ],
      "text": "arch"
    },
    {
      "rectangle": [
        [
          540,
          246
        ],
        [
          596,
          270
        ]
      ],
      "text": "stump"
    },
    {
      "rectangle": [
        [
          2,
          339
        ],
        [
          152,
          365
        ]
      ],
      "text": "2. lines of weakness"
    },
    {
      "rectangle": [
        [
          174,
          339
        ],
        [
          247,
          361
        ]
      ],
      "text": "sea cave"
    }
  ],
  "erosion_6852.png": [
    {
      "rectangle": [
        [
          20,
          103
        ],
        [
          45,
          132
        ]
      ],
      "text": "x"
    },
    {
      "rectangle": [
        [
          695,
          100
        ],
        [
          727,
          132
        ]
      ],
      "text": "y"
    },
    {
      "rectangle": [
        [
          369,
          372
        ],
        [
          575,
          425
        ]
      ],
      "text": "much fine material in suspension"
    },
    {
      "rectangle": [
        [
          27,
          281
        ],
        [
          172,
          309
        ]
      ],
      "text": "slip off slope"
    },
    {
      "rectangle": [
        [
          139,
          42
        ],
        [
          332,
          124
        ]
      ],
      "text": "sand and shingle deposited on inside of bend"
    },
    {
      "rectangle": [
        [
          632,
          342
        ],
        [
          714,
          393
        ]
      ],
      "text": "fastest current"
    },
    {
      "rectangle": [
        [
          406,
          43
        ],
        [
          635,
          135
        ]
      ],
      "text": "bank on outside of bend being undercut by lateral erosion"
    },
    {
      "rectangle": [
        [
          208,
          328
        ],
        [
          296,
          382
        ]
      ],
      "text": "slower current"
    },
    {
      "rectangle": [
        [
          629,
          19
        ],
        [
          739,
          46
        ]
      ],
      "text": "river cliff"
    }
  ],
  "erosion_6856.png": [
    {
      "rectangle": [
        [
          270,
          98
        ],
        [
          287,
          221
        ]
      ],
      "text": "eschooltoday.com"
    },
    {
      "rectangle": [
        [
          20,
          15
        ],
        [
          167,
          48
        ]
      ],
      "text": "weathering causes the rocks to break down"
    },
    {
      "rectangle": [
        [
          302,
          7
        ],
        [
          491,
          55
        ]
      ],
      "text": "erosion (water) and transport moves the sediments downhill to another place"
    }
  ],
  "erosion_6857.png": [
    {
      "rectangle": [
        [
          249,
          97
        ],
        [
          313,
          109
        ]
      ],
      "text": "overhang"
    },
    {
      "rectangle": [
        [
          255,
          201
        ],
        [
          331,
          217
        ]
      ],
      "text": "plunge pool"
    },
    {
      "rectangle": [
        [
          8,
          228
        ],
        [
          131,
          273
        ]
      ],
      "text": "steep-sided gorge develops as waterfall retreats"
    },
    {
      "rectangle": [
        [
          52,
          82
        ],
        [
          116,
          101
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          387,
          163
        ],
        [
          525,
          211
        ]
      ],
      "text": "ridges of hard rock create an uneven slope. this creates rapids."
    },
    {
      "rectangle": [
        [
          337,
          257
        ],
        [
          388,
          277
        ]
      ],
      "text": "soft rock"
    },
    {
      "rectangle": [
        [
          165,
          281
        ],
        [
          238,
          302
        ]
      ],
      "text": "fallen rocks"
    },
    {
      "rectangle": [
        [
          191,
          49
        ],
        [
          290,
          67
        ]
      ],
      "text": "waterfall retreats"
    },
    {
      "rectangle": [
        [
          308,
          287
        ],
        [
          365,
          307
        ]
      ],
      "text": "hard rock"
    }
  ],
  "erosion_6859.png": [
    {
      "rectangle": [
        [
          23,
          271
        ],
        [
          134,
          290
        ]
      ],
      "text": "lines of weakness"
    },
    {
      "rectangle": [
        [
          170,
          273
        ],
        [
          226,
          287
        ]
      ],
      "text": "sea cave"
    },
    {
      "rectangle": [
        [
          271,
          273
        ],
        [
          348,
          288
        ]
      ],
      "text": "undercutting"
    },
    {
      "rectangle": [
        [
          393,
          273
        ],
        [
          510,
          303
        ]
      ],
      "text": "wave-cut platform exposed at low tide"
    },
    {
      "rectangle": [
        [
          481,
          146
        ],
        [
          520,
          163
        ]
      ],
      "text": "stump"
    },
    {
      "rectangle": [
        [
          427,
          87
        ],
        [
          464,
          100
        ]
      ],
      "text": "stack"
    },
    {
      "rectangle": [
        [
          300,
          128
        ],
        [
          330,
          143
        ]
      ],
      "text": "arch"
    },
    {
      "rectangle": [
        [
          279,
          87
        ],
        [
          338,
          102
        ]
      ],
      "text": "headland"
    },
    {
      "rectangle": [
        [
          318,
          17
        ],
        [
          390,
          48
        ]
      ],
      "text": "site of arch collapse"
    },
    {
      "rectangle": [
        [
          446,
          18
        ],
        [
          532,
          46
        ]
      ],
      "text": "original shape of headland"
    }
  ],
  "erosion_6862.png": [
    {
      "rectangle": [
        [
          194,
          124
        ],
        [
          244,
          139
        ]
      ],
      "text": "stack"
    },
    {
      "rectangle": [
        [
          447,
          305
        ],
        [
          407,
          290
        ]
      ],
      "text": "arch"
    },
    {
      "rectangle": [
        [
          536,
          39
        ],
        [
          453,
          21
        ]
      ],
      "text": "blow hole"
    },
    {
      "rectangle": [
        [
          67,
          329
        ],
        [
          36,
          318
        ]
      ],
      "text": "sea"
    },
    {
      "rectangle": [
        [
          87,
          145
        ],
        [
          12,
          128
        ]
      ],
      "text": "high tide"
    },
    {
      "rectangle": [
        [
          331,
          356
        ],
        [
          261,
          340
        ]
      ],
      "text": "low tide"
    },
    {
      "rectangle": [
        [
          338,
          52
        ],
        [
          297,
          37
        ]
      ],
      "text": "cave"
    },
    {
      "rectangle": [
        [
          182,
          92
        ],
        [
          57,
          57
        ]
      ],
      "text": "stump covered at high tide"
    },
    {
      "rectangle": [
        [
          537,
          273
        ],
        [
          487,
          258
        ]
      ],
      "text": "caves"
    }
  ],
  "erosion_8064.png": [
    {
      "rectangle": [
        [
          11,
          226
        ],
        [
          128,
          279
        ]
      ],
      "text": "steep-sided gorge develops as waterfall retreats"
    },
    {
      "rectangle": [
        [
          304,
          292
        ],
        [
          365,
          308
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          194,
          50
        ],
        [
          292,
          70
        ]
      ],
      "text": "waterfall retreats"
    },
    {
      "rectangle": [
        [
          391,
          164
        ],
        [
          523,
          212
        ]
      ],
      "text": "ridges of hard rock create an uneven slope. this creates rapids."
    },
    {
      "rectangle": [
        [
          55,
          84
        ],
        [
          113,
          101
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          170,
          282
        ],
        [
          239,
          300
        ]
      ],
      "text": "fallen rocks"
    },
    {
      "rectangle": [
        [
          252,
          197
        ],
        [
          330,
          225
        ]
      ],
      "text": "plunge pool"
    },
    {
      "rectangle": [
        [
          253,
          92
        ],
        [
          315,
          113
        ]
      ],
      "text": "overhang"
    },
    {
      "rectangle": [
        [
          337,
          260
        ],
        [
          389,
          279
        ]
      ],
      "text": "soft rock"
    }
  ],
  "erosion_8066.png": [
    {
      "rectangle": [
        [
          196,
          12
        ],
        [
          382,
          34
        ]
      ],
      "text": "(4) waterfall retreats upstream"
    },
    {
      "rectangle": [
        [
          85,
          97
        ],
        [
          167,
          126
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          87,
          182
        ],
        [
          166,
          208
        ]
      ],
      "text": "soft rock"
    },
    {
      "rectangle": [
        [
          41,
          238
        ],
        [
          139,
          268
        ]
      ],
      "text": "(1) undercutting"
    },
    {
      "rectangle": [
        [
          338,
          81
        ],
        [
          478,
          103
        ]
      ],
      "text": "(2) overhang collapses"
    },
    {
      "rectangle": [
        [
          414,
          158
        ],
        [
          582,
          183
        ]
      ],
      "text": "(5) steep, gorge-like valleys"
    },
    {
      "rectangle": [
        [
          334,
          224
        ],
        [
          483,
          245
        ]
      ],
      "text": "(3) plunge pool develops"
    },
    {
      "rectangle": [
        [
          224,
          318
        ],
        [
          423,
          338
        ]
      ],
      "text": "formation of a waterfall"
    }
  ],
  "erosion_8067.png": [
    {
      "rectangle": [
        [
          121,
          123
        ],
        [
          63,
          106
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          240,
          255
        ],
        [
          175,
          238
        ]
      ],
      "text": "plunge pool"
    },
    {
      "rectangle": [
        [
          418,
          146
        ],
        [
          347,
          125
        ]
      ],
      "text": "overhang"
    },
    {
      "rectangle": [
        [
          227,
          32
        ],
        [
          107,
          14
        ]
      ],
      "text": "waterfall retreats"
    },
    {
      "rectangle": [
        [
          256,
          338
        ],
        [
          172,
          318
        ]
      ],
      "text": "fallen rocks"
    }
  ],
  "erosion_8068.png": [
    {
      "rectangle": [
        [
          318,
          283
        ],
        [
          487,
          322
        ]
      ],
      "text": "hard rock"
    },
    {
      "rectangle": [
        [
          173,
          555
        ],
        [
          478,
          613
        ]
      ],
      "text": "(1) undercutting"
    },
    {
      "rectangle": [
        [
          270,
          458
        ],
        [
          453,
          507
        ]
      ],
      "text": "soft rock"
    },
    {
      "rectangle": [
        [
          205,
          560
        ],
        [
          253,
          605
        ]
      ],
      "text": "(1)"
    },
    {
      "rectangle": [
        [
          255,
          560
        ],
        [
          433,
          607
        ]
      ],
      "text": "undercutting"
    },
    {
      "rectangle": [
        [
          255,
          450
        ],
        [
          448,
          502
        ]
      ],
      "text": "soft rock"
    },
    {
      "rectangle": [
        [
          198,
          550
        ],
        [
          438,
          613
        ]
      ],
      "text": "(1) undercutting"
    }
  ]
}
## tip5
- instructionalDiagrams
    
    - diagram name:
        - "imagePath": relative path to image file from the dataset root directory.
        - "imageName": name of the diagram image file,
        - "rawText": human written description of diagram,
        - "processedText": normalized text of the description
{
  "DD_0001": {
    "globalID": "DD_0001",
    "imageName": "erosion_6859.png",
    "imagePath": "teaching_images/erosion_6859.png",
    "processedText": null
  }
}
