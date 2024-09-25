# Description
## Skills
| Field      | Annotation                     | Example |
| ---------- | ------------------------------ | ------- |
| id         | id of the skill                | 1870    |
| identifier | string identifier of the skill | numbers |
| name       |  czech name of the skill       | očítání |
| parent     | parent skill id                | 1869    |
The skills are organized in a tree structure. Note that only some of _the level 2 skills_ have children.
![[Pasted image 20240924200641.png]]
## Items
Every item belongs to exactly one skill (mostly level 2 or level 3 skills). Features 'skill_lvl_X' stands for ancestor skill of item on given level. They can be used for comfortable item filtering.

| Field         | Annotation                                       | Example                       |
| ------------- | ------------------------------------------------ | ----------------------------- |
| id            | the id of the item                               | 1                             |
| question      | human readable question represented by item      | 1                             |
| answer        | human readable correct answer to item            | 1                             |
| visualization | type of visualization of question[[MatMat#Tip1]] | object_selection_answer       |
| skill         | the smallest skill containing the item           | 1873                          |
| skill_lvl_1   | skill on the level 1 containing the item         | 1870                          |
| skill_lvl_2   | skill on the level 2 containing the item         | 1871                          |
| skill_lvl_3   | skill on the level 3 containing the item         | 1873                          |
| data          | JSON with information about question and answer  | "{'answer':1,'operands':[1]}" |
## Answer
| Field           | Annotation                                                                                                                        | Example                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| id              | id of the answer                                                                                                                  | 273951                                                                                                              |
| time            | time of the answer                                                                                                                | 2016-04-17 14:12:09                                                                                                 |
| item            | id of the item                                                                                                                    | 38                                                                                                                  |
| student         | id of the user                                                                                                                    | 33480                                                                                                               |
| sessions        | id of user's session                                                                                                              |                                                                                                                     |
| response_time   | time taken to answer an item in milliseconds                                                                                      | 57276                                                                                                               |
| correct         | 0 for incorrect answer and 1 for correct answer                                                                                   | 0                                                                                                                   |
| answer          | answer given by the user                                                                                                          | 14                                                                                                                  |
| answer_expected |  expected answer                                                                                                                  | 13                                                                                                                  |
| log             | JSON with addition information about answer<br><br>- device used by the user<br>- log of the user actions during solving the item | "{""client_meta"": [[11382, ""soft-keyboard:3""], [11382, ""3""], [17068, ""finished""]], ""device"": ""desktop""}" |
| random          | 0 for adaptively selected items and 1 randomly selected items                                                                     | 0                                                                                                                   |
# Tip1
![[Pasted image 20240924202336.png]]
![[Pasted image 20240924202347.png]]
![[Pasted image 20240924202357.png]]![[Pasted image 20240924202405.png]]
![[Pasted image 20240924202424.png]]
![[Pasted image 20240924202435.png]]
![[Pasted image 20240924202445.png]]