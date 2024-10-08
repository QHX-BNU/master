# Description
| Field         | Annotation                                                                                                                                                                                                                                                                                                 | Example                                                  |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| id            | a unique 10-bytes character identifier                                                                                                                                                                                                                                                                     | nluds-0001                                               |
| Grade         | a grade level indicating the level of difficulty                                                                                                                                                                                                                                                           | 1                                                        |
| Source        | an url identifying the reference source where the MWP(Math Word Problem) came from                                                                                                                                                                                                                         | http://www.k5learning.com                                |
| Body          | the problem text includes facts and clues for solving an MWP                                                                                                                                                                                                                                               | Seven red apples and two green apples are in the basket. |
| Question      | the text identify the question to solve.                                                                                                                                                                                                                                                                   | How many apples are in the basket?                       |
| Solution-Type | a tag which indicates a crucial math operation pattern for solving an MWP. Currently, we provide 24 different common solution types. Details are shown in our paper.[A Diverse Corpus for Evaluating and Developing English Math Word Problem Solvers](https://www.aclweb.org/anthology/2020.acl-main.92/) | Addition                                                 |
| Answer        | the annodated answer (includes associated measurement units if exists)                                                                                                                                                                                                                                     | 9 (apples)                                               |
| Formula       | the annotated formula                                                                                                                                                                                                                                                                                      | 7+2=9                                                    |
# Tip1
![[Pasted image 20240929103754.png]]
For multiple-step MWPs, the formula can be represented as an expression tree. The non-leaf nodes are operations and the leaf-nodes are operands. We denote the operation in the **root node** to be the **Solution-type** of this MWP, and the other operations on the non-leaf nodes are sub-types (in a depth-first travel manner) of the MWP and are denoted in the **Subtype** attribute of the **Solution-type**.