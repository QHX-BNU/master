# Description

| Field          | Annotation                               | Example                                                                                  |
| -------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------- |
| id             | Id of the problem                        | 946                                                                                      |
| original_text  | Original text of the problem             | 甲数除以乙数的商是1.5，如果甲数增加20，则甲数是乙的4倍．原来甲数=．                                                    |
| equation       | Solution to the problem                  | x=20/(4-1.5)*1.5                                                                         |
| segmented_text | Chinese word segmentation of the problem | 从 甲地 到 乙地 ， 如果 骑 自行车 每 小时 行驶 16 千米 ， 4 小时 可以 到达 ， 如果 乘 汽车 只 需要 2 小时 ， 汽车 每 小时 行驶 多少 千米 ？ |
| ans            | the answer to the problem                | 32                                                                                       |
只有问题文本，没有学生的交互数据