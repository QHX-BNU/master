https://github.com/riiid/ednet?tab=readme-ov-file
https://arxiv.org/pdf/1912.03072
![[Pasted image 20240917211613.png]]

It aims to prepare students for the TOEIC (Test of English for International Communication R ) Listening and Reading Test
# Description
KT1 consists of students' question-solving logs, which is the most basic and fundamental information that can be used by various deep-learning knowledge tracing models such as Deep Knowledge Tracing and Self-Attentive Knowledge Tracing. EdNet-KT1 is the record of _Santa_ collected since Apr 18. 2017 following this question-response sequence format. A major property of EdNet is that the questions come in _bundles_. That is, a collection of questions sharing a common passage, picture or listening material. For example, questions of ID `q2319`, `q2320` and `q2321` may share the same reading passage. In this case, the questions are said to form a bundle and will be given to the student with corresponding shared material. When a bundle is given, a student have access to all the problems and has to respond all of them in order to complete the bundle.

| Field        | Annotation                                                                                                              | Example       |
| ------------ | ----------------------------------------------------------------------------------------------------------------------- | ------------- |
| user_id      | student’s id                                                                                                            | u717875       |
| timestamp    | the moment the question was given, represented as Unix timestamp in milliseconds                                        | 1565332027449 |
| solving_id   | represents each learning session of students corresponds to each bunle. It is a form of single integer, starting from 1 | 1             |
| question_id  | the ID of the question that given to student, which is a form of q{integer}                                             | q4862         |
| user_answer  | the answer that the student submitted, recorded as a character between a and d inclusively                              | a(选择题？)       |
| elapsed_time | the time that the students spends on each question in milliseconds                                                      | 45000         |
