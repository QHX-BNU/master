https://raw.githubusercontent.com/hyDududu/FlaCGEC

# Description
| Field      | Annotation                      | Example                                                                                                    |
| ---------- | ------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| id         | the id of the sentence          | 0                                                                                                          |
| source     | the source of the sentence      | 母亲说：“写完院里那样18缸水，你的字会有筋骨、有血肉。”                                                                              |
| target     | the target of the sentence      | 母亲说：“写完院里这18缸水，你的字才会有筋骨、有血肉。”                                                                              |
| operation  | the operation of the sentence   | [[(9, 10, '那样'), '指示代词', 'S', ('null', 'null', '这')], [(19, 19, '会'), '语气副词', 'M', ('null', 'null', '才')]] |
| annotation | the annotation of the operation | 9 10\|\|\|S-指示代词\|\|\|这;19 19\|\|\|M-语气副词\|\|\|才                                                           |