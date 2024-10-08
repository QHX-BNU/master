https://raw.githubusercontent.com/xlxwalex/FCGEC

# Description
| Field      | Annotation                                                              | Example                                                                                                                                                                                        |
| ---------- | ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id         | the id of the sentence                                                  | 9d1124f5e0213001f8e16816e40bb1fa                                                                                                                                                               |
| sentence   | the text of the sentence                                                | 由于加强了生产过程中的生态环境监控，该基地每年的无公害蔬菜的生产量除供应本省主要市场外，还销往河南、河北等省。                                                                                                                                        |
| error_flag | Whether sentence contains errors(0 or 1)                                | 1                                                                                                                                                                                              |
| error_type | The error types of sentence / 原句的错误类型，若为非病句则为*[[FCGEC#Task]]            | IWC                                                                                                                                                                                            |
| operation  | he operation of the  reference /编辑操作的json字符串"[[FCGEC#Opetation format]] | [{\"Switch\":[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,30,31,23,24,25,26,27,28,29,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54],\"Delete\":[31,32]}] |
| external   | Additional information (e.g., version) / 额外信息                           | FCGEC EMNLP 2022                                                                                                                                                                               |




# Task
- _**错误检测 (error detection)：**_ 模型需要判断给定的句子是否包含语法错误 (二分类任务)
- _**类型检测 (type identification)：**_ 模型需要判定句子中的语法错误属于七种错误类型中的哪一种，错误类型分别为：
    1. 语序不当 (Incorrect Word Order, IWO)
    2. 搭配不当 (Incorrect Word Collocation, IWC)
    3. 成分缺失 (Component Missing, CM)
    4. 成分赘余 (Component Redundancy, CR)
    5. 结构混乱 (Structure Confusion, SC)
    6. 不合逻辑 (Illogical, ILL)
    7. 语意不明 (Ambiguity, AM)
- _**文本纠错 (error correction)：**_ 给定一个句子，模型输出对应的无语法错误句子

# Opetation format
Suppose the given sentence is "A B C D E".

假设原始句子是 “A B C D E”

### 1. Switch operation（交换操作）

[](https://github.com/xlxwalex/FCGEC/blob/main/data/README.md#1-switch-operation%E4%BA%A4%E6%8D%A2%E6%93%8D%E4%BD%9C)

```json
{"Switch":[0,2,1,3,4]}                               // (A B C D E → A C B D E)
```

### 2. Delete operation（删除操作）

[](https://github.com/xlxwalex/FCGEC/blob/main/data/README.md#2-delete-operation%E5%88%A0%E9%99%A4%E6%93%8D%E4%BD%9C)

```json
{"Delete":[3]}                                       // (A B C D E → A B C E)
```

### 3. Insert operation（插入操作）

[](https://github.com/xlxwalex/FCGEC/blob/main/data/README.md#3-insert-operation%E6%8F%92%E5%85%A5%E6%93%8D%E4%BD%9C)

```json
{"Insert":[{"pos":1,"tag":"INS_1","label":["F"]}]}  // (A B C D E → A B F C D E)
```

### 4. Modify operation（修改操作）

[](https://github.com/xlxwalex/FCGEC/blob/main/data/README.md#4-modify-operation%E4%BF%AE%E6%94%B9%E6%93%8D%E4%BD%9C)

```json
{"Modify":[{"pos":2,"tag":"MOD_1","label":["F"]}]}  // (A B C D E → A B F D E)
```