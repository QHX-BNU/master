# Download
Reading Comprehension for Traditional Chinese<br>
https://huggingface.co/datasets/clue/clue
https://github.com/CLUEbenchmark/

# Description
| Field   | Annotation              | Example       |
| ------- | ----------------------- | ------------- |
| version | the version of the task | 1.3           |
| data    | the data of the task    | [[DRCD#data]] |
## data
| Field      | Annotation                           | Example             |
| ---------- | ------------------------------------ | ------------------- |
| title      | the title of the passage             | 基督新教                |
| id         | the id of the passage                | 2128                |
| paragraphs | the text and question of the context | [[DRCD#paragraphs]] |
### paragraphs
| Field   | Annotation                  | Example                                                                                                                                                                                                                                                                                                   |
| ------- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| context | the title of the paragraphs | 基督新教與天主教均繼承普世教會歷史上許多傳統教義，如三位一體、聖經作為上帝的啟示、原罪、認罪、最後審判等等，但有別於天主教和東正教，新教在行政上沒有單一組織架構或領導，而且在教義上強調因信稱義、信徒皆祭司， 以聖經作為最高權威，亦因此否定以教宗為首的聖統制、拒絕天主教教條中關於聖傳與聖經具同等地位的教導。新教各宗派間教義不盡相同，但一致認同五個唯獨：唯獨恩典：人的靈魂得拯救唯獨是神的恩典，是上帝送給人的禮物。唯獨信心：人唯獨藉信心接受神的赦罪、拯救。唯獨基督：作為人類的代罪羔羊，耶穌基督是人與上帝之間唯一的調解者。唯獨聖經：唯有聖經是信仰的終極權威。唯獨上帝的榮耀：唯獨上帝配得讚美、榮耀 |
| id      | the id of the paragraphs    | 2128-2                                                                                                                                                                                                                                                                                                    |
| qas     | the question of the context | [[DRCD#qas]]                                                                                                                                                                                                                                                                                              |
#### qas
| Field    | Annotation               | Example                                             |
| -------- | ------------------------ | --------------------------------------------------- |
| id       | the id of the query      | 2128-2-1                                            |
| question | the text of the query    | 新教在教義上強調信徒皆祭司以及什麼樣的理念?                              |
| answers  | the answers to the query | "id": "1",<br>"text": "因信稱義",<br>"answer_start": 92 |
