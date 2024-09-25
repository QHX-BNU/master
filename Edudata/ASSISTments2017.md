# 1.Description
| Field                                  | Annotation                                                                                                                                                                                    | Example                         |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- |
| student id/ITEST id                    | a deidentified ID/tag used for identifying an individual student                                                                                                                              | 8                               |
| SY ASSISTments Usage                   | the academic years the student used ASSISTments(这个测试数据是在哪一年测试产生的，有不同的年份)                                                                                                                      | 2004-2005                       |
| AveKnow                                | average student knowledge level (according to Bayesian Knowledge Tracing algorithm – cf. Corbett & Anderson, 1995[[ASSISTments2017#tip1]] )                                                   | 0.352416                        |
| AveCarelessness                        | average student carelessness (according to San Pedro, Baker, & Rodrigo, 2011 model[[ASSISTments2017#tip2]])                                                                                   | 0.183276                        |
| AveCorrect                             | average student correctness<br>                                                                                                                                                               | 0.483902                        |
| NumActions                             | total number of student actions in system                                                                                                                                                     | 1056                            |
| AveResBored                            | average student affect: boredom (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014)                                                                                                          | 0.208389                        |
| AveResEngcon                           | average student affect:engaged concentration (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014)                                                                                             | 0.679126                        |
| AveResConf                             | average student affect:confusion (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014)                                                                                                         | 0.115905                        |
| AveResFrust                            | average student affect:frustration (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014)                                                                                                       | 0.112408                        |
| AveResOfftask                          | average student affect: off task (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014 and also Baker, 2007)                                                                                    | 0.156503                        |
| AveResGaming                           | average student affect:gaming the system (see Pardos, Baker, San Pedro, Gowda, & Gowda, 2014 and also Baker Corbett Koedinger & Wagner, 2004)                                                 | 0.196561                        |
| actionId                               | the unique id of this specific action[[#tip3]]                                                                                                                                                | 9950                            |
| skill                                  | a tag used for identifying the cognitive skill related to the problem (see Razzaq, Heffernan, Feng, & Pardos, 2007)[[#tip4]]                                                                  | properties-of-geometric-figures |
| problemId                              | a unique ID used for identifying a single problem                                                                                                                                             | 1118                            |
| assignmentId                           | a unique ID used for identifying an assignment                                                                                                                                                | 20405010                        |
| assistmentId                           | a unique ID used for identifying an assistment (a instance of a multi-part problem)                                                                                                           | 104051118                       |
| startTime                              | when did the student start the problem (UNIX time, seconds)                                                                                                                                   | 1096470301                      |
| endTime                                | when did the student end the problem (UNIX time, seconds)                                                                                                                                     | 1096470350                      |
| timeTaken                              | Time spent on the current step                                                                                                                                                                | 49                              |
| correct                                | Answer is correct                                                                                                                                                                             | 0                               |
| original                               | Problem is original not a scaffolding problem                                                                                                                                                 | 1                               |
| hint                                   | Action is a hint response                                                                                                                                                                     | 1                               |
| hintCount                              | Total number of hints requested so far                                                                                                                                                        | 1                               |
| hintTotal                              | Total number of hints requested for the problem                                                                                                                                               | 1                               |
| scaffold                               | Problem is a scaffolding problem                                                                                                                                                              | 0                               |
| bottomHint                             | Bottom-out hint is used[[questions#2]]                                                                                                                                                        | 0                               |
| attemptCount                           | Total problems attempted in the tutor so far.                                                                                                                                                 | 1                               |
| problemType                            | the type of the problem[[#tip5]]                                                                                                                                                              | textfieldquestion               |
| frIsHelpRequest                        | First response is a help request                                                                                                                                                              | 1                               |
| frPast5HelpRequest                     | Number of last 5 First responses that included a help request[[#tip6]]                                                                                                                        | 0                               |
| frPast8HelpRequest                     | Number of last 8 First responses that included a help request                                                                                                                                 | 0                               |
| stlHintUsed                            | Second to last hint is used an indicates a hint that gives considerable detail but is not quite bottom-out                                                                                    | 0                               |
| past8BottomOut                         | Number of last 8 problems that used the bottom-out hint.                                                                                                                                      | 0                               |
| totalFrPercentPastWrong                | Percent of all past problems that were wrong on this KC.                                                                                                                                      | 0                               |
| totalFrPastWrongCount                  | Total first responses wrong attempts in the tutor so far.                                                                                                                                     | 0                               |
| frPast5WrongCount                      | Number of last 5 First responses that were wrong                                                                                                                                              | 0                               |
| frPast8WrongCount                      | Number of last 8 First responses that were wrong                                                                                                                                              | 0                               |
| totalFrTimeOnSkill                     | Total first response time spent on this KC across all problems                                                                                                                                | 0                               |
| timeSinceSkill                         | Time since the current KC was last seen.                                                                                                                                                      | 0                               |
| frWorkingInSchool                      | First response Working during school hours (between 7:00 am and 3:00 pm)                                                                                                                      | 1                               |
| totalFrAttempted                       | Total first responses attempted in the tutor so far.                                                                                                                                          | 3                               |
| totalFrSkillOpportunities              | Total first response practice opportunities on this KC so far.                                                                                                                                | 0                               |
| responseIsFillIn                       | Response is filled in (No list of answers available)                                                                                                                                          | 0                               |
| responseIsChosen                       | Response is chosen from a list of answers (Multiple choice, etc).                                                                                                                             | 0                               |
| endsWithScaffolding                    | Problem ends with scaffolding                                                                                                                                                                 | 0                               |
| endsWithAutoScaffolding                | Problem ends with automatic scaffolding                                                                                                                                                       | 0                               |
| frTimeTakenOnScaffolding               | First response time taken on scaffolding problems                                                                                                                                             | 0                               |
| frTotalSkillOpportunitiesScaffolding   | Total first response practice opportunities on this skill so far                                                                                                                              | 0                               |
| totalFrSkillOpportunitiesByScaffolding | Total first response scaffolding opportunities for this KC so far                                                                                                                             | 0                               |
| frIsHelpRequestScaffolding             | First response is a help request Scaffolding                                                                                                                                                  | 0                               |
| timeGreater5Secprev2wrong              | Long pauses after 2 Consecutive wrong answers                                                                                                                                                 | 0                               |
| sumRight                               | NaN[[#tip7]]                                                                                                                                                                                  | 0                               |
| helpAccessUnder2Sec                    | Time spent on help was under 2 seconds                                                                                                                                                        | 0                               |
| timeGreater10SecAndNextActionRight     | Long pause after correct answer                                                                                                                                                               | 0                               |
| consecutiveErrorsInRow                 | Total number of 2 wrong answers in a row across all the problems                                                                                                                              | 0                               |
| sumTime3SDWhen3RowRight                | NaN                                                                                                                                                                                           | 0                               |
| sumTimePerSkill                        | NaN                                                                                                                                                                                           | 49                              |
| totalTimeByPercentCorrectForskill      | Total time spent on this KC across all problems divided by percent correct for the same KC                                                                                                    | 0                               |
| prev5count                             | NaN                                                                                                                                                                                           | 0                               |
| timeOver80                             | NaN                                                                                                                                                                                           | 0                               |
| manywrong                              | NaN                                                                                                                                                                                           | 0                               |
| confidence(BORED)                      | the confidence of the student affect prediction: bored                                                                                                                                        | 0.59786477                      |
| confidence(CONCENTRATING)              | the confidence of the student affect prediction: concecntrating                                                                                                                               | 0.23429359                      |
| confidence(CONFUSED)                   | the confidence of the student affect prediction: confused                                                                                                                                     | 0                               |
| confidence(FRUSTRATED)                 | the confidence of the student affect prediction: frustrated                                                                                                                                   | 0                               |
| confidence(OFF TASK)                   | the confidence of the student affect prediction: off task                                                                                                                                     | 0.83870968                      |
| confidence(GAMING)                     | the confidence of the student affect prediction: gaming                                                                                                                                       | 0.00852182                      |
| RES_BORED                              | rescaled of the confidence of the student affect prediction: boredom                                                                                                                          | 0.37642746                      |
| RES_CONCENTRATING                      | rescaled of the confidence of the student affect prediction: concentration                                                                                                                    | 0.32031737                      |
| RES_CONFUSED                           | rescaled of the confidence of the student affect prediction confusion                                                                                                                         | <br>0                           |
| RES_FRUSTRATED                         | rescaled of the confidence of the student affect prediction:frustration                                                                                                                       | 0                               |
| RES_OFFTASK                            | rescaled of the confidence of the student affect prediction: off task                                                                                                                         | 0.78558547                      |
| RES_GAMING                             | rescaled of the confidence of the student affect prediction: gaming                                                                                                                           | 0.0002642                       |
| Ln-1                                   | baysian knowledge tracing’s knowledge estimate at the previous time step                                                                                                                      | 0.13                            |
| Ln                                     | baysian knowledge tracing’s knowledge estimate at the time step                                                                                                                               | 0.06119041                      |
| schoolID                               | the id (anonymized) of the school the student was in during the year the data was collected                                                                                                   | 1                               |
| MCAS                                   | Massachusetts Comprehensive Assessment System test score. In short, this number is the student’s state test score (outside ASSISTments) during that year. -999 represents the data is missing | 45                              |
| Enrolled[[ASSISTments2017#tip9]]       |                                                                                                                                                                                               | 0                               |
| Selective                              |                                                                                                                                                                                               | 0                               |
| isSTEM                                 |                                                                                                                                                                                               | NaN                             |

## tip1
初始概率通过实验或者专家评定确定
![](image/Pasted image 20240913152907.png)

![[Pasted image 20240913152940.png]]
## tip2

Title::Improving Contextual Models of Guessing and Slipping with a Truncated Training Set
![[Pasted image 20240913174821.png]]
上述$L_{n}$表示在第n次测试中学生掌握该知识的概率
![[Pasted image 20240913175810.png]]
## tip3
暂且存疑
![[Pasted image 20240914092407.png]]

## tip4
是否表示知识的水平：知道，应用，分析，综合，创新
![[Pasted image 20240914113909.png]]

properties-of-geometric-figures
application:Isosceles triangle
有几种类型？
## tip5
有几种problemtype
## tip6
什么是first response
## tip7
???NaN
## tip8
全部正确预计的时间？？？
## tip9
后面三行什么意思？？
