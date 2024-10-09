# Download
蚂蚁金融语义相似度 Ant Financial Question Matching Corpus<br>
https://huggingface.co/datasets/clue/clue<br>
https://github.com/CLUEbenchmark

# Description
| Field     | Annotation                                                              | Example   |
| --------- | ----------------------------------------------------------------------- | --------- |
| sentence1 | a `string` feature                                                      | 双十一花呗提额在哪 |
| sentence2 | a `string` feature                                                      | 里可以提花呗额度  |
| label     | a classification label, with possible values including `0` (0), `1` (1) | 0         |
| idx       | a `int32` feature， the ID                                               | 0         |
***notice***:```
每一条数据有三个属性，从前往后分别是 句子1，句子2，句子相似度标签。其中label标签，1 表示sentence1和sentence2的含义类似，0表示两个句子的含义不同。
