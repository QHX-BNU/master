https://huggingface.co/datasets/RUCAIBox/gaokao-bench

# Description
| Field    | Annotation                                                                    | Example                                                                                                                               |
| -------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| year     | the year of the gaokao exam                                                   | 2010                                                                                                                                  |
| category | the categoty of the exam                                                      | （新课标）                                                                                                                                 |
| question | the text of the question ,  if it is choice question, it will include choices | 1．（ 6分）下列有关细胞的叙述，正确的是（ 　　） A．病毒是一类具有细胞结构的生物 B．蓝藻细胞具有细胞核且 DNA分子呈环状 C．人体所有细胞的细胞周期持续时间相同 D．内质网膜和高尔基体膜都具有流动性                              |
| answer   | the answer to the question                                                    | D                                                                                                                                     |
| analysis | the analysis of the question                                                  | 解： A、病毒是不具有细胞结构的生物， A错误； B、蓝藻属于原核生物，原核细胞内无细胞核， B错误； C、人体的不同组织 ，细胞分裂的速度不同 ，细胞周期持续的时间不同 ，C错误； D、内质网膜与高尔基体膜与细胞膜的结构相似，都具有流动性， D正确。 故选： D。 |
| index    | the index of the question                                                     | 0                                                                                                                                     |
| score    | the score of the question                                                     | 6                                                                                                                                     |