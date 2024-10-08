https://huggingface.co/datasets/clue/clue
https://github.com/CLUEbenchmark/CLUE

 Short Text Classificaiton for News

# Description
| Field     | Annotation  | Example                    |
| --------- | ----------- | -------------------------- |
| sentence  | 新闻字符串（仅含标题） | 江疏影甜甜圈自拍，迷之角度竟这么好看，美吸引一切事物 |
| label     | 句子标签ID      | 102                        |
| label_des | 标签名称        | news_entertainment         |
***notice***:该数据集来自今日头条的新闻版块，共提取了15个类别的新闻，包括旅游，教育，金融，军事等。每一条数据有三个属性，从前往后分别是 分类ID，分类名称，新闻字符串（仅含标题）。