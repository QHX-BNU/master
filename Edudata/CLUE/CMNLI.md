# Download
https://huggingface.co/datasets/clue/clue
https://github.com/CLUEbenchmark/

被OCNLI替代

# Description
| Field     | Annotation                                                                       | Example      |
| --------- | -------------------------------------------------------------------------------- | ------------ |
| sentence1 | the first sentence                                                               | 新的权利已经足够好了   |
| sentence2 | the second sentence                                                              | 每个人都很喜欢最新的福利 |
| label     | 每一条数据有三个属性，从前往后分别是 句子1，句子2，蕴含关系标签。其中label标签有三种：neutral，entailment，contradiction。 | neutral      |
***notice***
CMNLI数据由两部分组成：XNLI和MNLI。数据来自于fiction，telephone，travel，government，slate等，对原始MNLI数据和XNLI数据进行了中英文转化，保留原始训练集，合并XNLI中的dev和MNLI中的matched作为CMNLI的dev，合并XNLI中的test和MNLI中的mismatched作为CMNLI的test，并打乱顺序。该数据集可用于判断给定的两个句子之间属于蕴涵、中立、矛盾关系。
