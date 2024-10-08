https://huggingface.co/datasets/clue/clue
https://github.com/CLUEbenchmark/CLUE

# Description
| Field     | Annotation                                                                       | Example             |
| --------- | -------------------------------------------------------------------------------- | ------------------- |
| sentence1 | the first sentence                                                               | 身上裹一件工厂发的棉大衣,手插在袖筒里 |
| sentence2 | the second sentence                                                              | 身上至少一件衣服            |
| label     | 每一条数据有三个属性，从前往后分别是 句子1，句子2，蕴含关系标签。其中label标签有三种：neutral，entailment，contradiction。 | entailment          |
| level     | the level of the task                                                            | medium              |
| genre     | the genre of the sentence                                                        | lit                 |
| prem_id   | the id of the task                                                               | lit_635             |
| id        | the id of the task                                                               | 0                   |