# Download
https://www.fi.muni.cz/adaptivelearning/?a=data

# Description
## Skills
| Field      | Annotation                     | Example |
| ---------- | ------------------------------ | ------- |
| id         | id of the skill                | 1870    |
| identifier | string identifier of the skill | numbers |
| name       |  czech name of the skill       | očítání |
| parent     | parent skill id                | 1869    |

The skills are organized in a tree structure. Note that only some of _the level 2 skills_ have children.
![Pasted image 20240924200641](https://github.com/user-attachments/assets/91c02364-4753-4ff8-a56b-4bf0624f384e)

## Items
Every item belongs to exactly one skill (mostly level 2 or level 3 skills). Features 'skill_lvl_X' stands for ancestor skill of item on given level. They can be used for comfortable item filtering.

| Field         | Annotation                                       | Example                       |
| ------------- | ------------------------------------------------ | ----------------------------- |
| id            | the id of the item                               | 1                             |
| question      | human readable question represented by item      | 1                             |
| answer        | human readable correct answer to item            | 1                             |
| visualization | [type of visualization of question](#Tip1) | object_selection_answer       |
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
![Pasted image 20240924202336](https://github.com/user-attachments/assets/8cd9bdd2-1d0d-445f-9b57-90d3624e8cc9)

![Pasted image 20240924202347](https://github.com/user-attachments/assets/bf3ec03c-bc51-4de5-a445-009541083f76)

![Pasted image 20240924202357](https://github.com/user-attachments/assets/8911f6b7-37ee-43c6-b4d6-3da0779001a5)
![Pasted image 20240924202405](https://github.com/user-attachments/assets/d54bf7c9-5e4a-4dc8-938b-f280f1d85fde)

![Pasted image 20240924202424](https://github.com/user-attachments/assets/b9afc47e-78c9-4784-909c-081519cc413f)

![Pasted image 20240924202435](https://github.com/user-attachments/assets/76c63627-7d7f-4d7b-a816-62aa1081e1da)

![Pasted image 20240924202445](https://github.com/user-attachments/assets/b60e4c24-2c56-4f3d-9a97-7ed5abb6f6c7)
