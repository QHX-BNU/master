https://www.microsoft.com/en-us/research/uploads/prod/2015/08/dolphin18k.pdf
数据库下载：
https://github.com/nexuslrf/NLP_MathWordProblem/blob/master/data/
Dolphin18K is a dataset created for math word problem solving, containing 18,460 problems posted by users on the community question answering site, Yahoo! Answers.

# Description
| Field         | Annotation                                                                  | Example                                                                                      |
| ------------- | --------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| id            | Unique id of a problem.                                                     | yahoo.answers. 20061213041448AAxoy5z                                                         |
| original text | Original problem text from yahoo answer.                                    | what is 30 divided by half plus 10? 1st correct answer gets 10 points!!!!!?\n（目前找到的数据库这一项为空） |
| text          | Cleaned problem text by removing problem unrelated text, used in our paper. | what is 30 divided by half plus 10? ~~1st correct answer gets 10 points!!!!!?\n~~            |
| equations     | The equations used to solve the problem.[[Dolphin18K#Tip1]]                 | unkn: x equ: x=30/(1/2)+10                                                                   |
| ans           | Problem answer                                                              | 70                                                                                           |
| flag          | Annotation status of the problem                                            | 0 – annotation done                                                                          |
# Tip1
## Equation annotation
1. "unkn":the variables whose values will be problem answers
2. “equ”: the first equation
3. “equ”: the second equation
4. ......
5. “equ”: the last equation

## Answer annotation
1. “;”: separate the values of different variables.
2. “{}”: any order of variables is allowed.
3. “|”: different answer formats.
4. “or”: different solutions to the problem.
![Pasted image 20240925085329](https://github.com/user-attachments/assets/23e8cd23-58fa-48a9-95e5-09b84ea5498a)

