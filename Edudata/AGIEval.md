# Download
https://github.com/ruixiangcui/AGIEval

# Paper
This dataset is for paper [AGIEval: A Human-Centric Benchmark for Evaluating Foundation Models](https://arxiv.org/abs/2304.06364)

# Description
| Field    | Annotation                                                      | Example                                                                                                                                                                                                                                                      |
| -------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| passage  | the passage of the question                                     | 天嚣。风，像浪一样，梗着头向钢架房冲撞。钢架房,便发疟疾般地一阵阵战栗、摇晃，像是随时都要散架...(文章太长所以省略后文)                                                                                                                                                                                               |
| question | the text of the question                                        | 下列对小说相关内容和艺术特色的分析鉴赏，不正确的一项是                                                                                                                                                                                                                                  |
| options  | the options of the question                                     | (A)小说开头不仅形象地描写了风沙的狂暴，也细致地表现了人物的直觉印象与切身感受，烘托并渲染了“”天气“恐怖气氛。<br>(B)被困队员身陷绝境却调动起所有能量开门救助敲门人，送瓜人在被困队员生死关头奇迹般的出现，这都说明生命奇迹无法解释。<br>(C)小说善于运用细节表现人物，开门前试验队员一句“桌子上有资料没有？当心被风卷进去”，就体现了科研工作者高度的责任意识。<br>(D)试验队被困队员与素不相识的送瓜人之间的故事，不仅令人感动，还揭示出一个朴素而有意味的人生道理：帮助别人，也是帮助自己。" |
| label    | The answer for multi-choice tasks is saved in the `label` field | B                                                                                                                                                                                                                                                            |
| answer   | The answer for cloze tasks is saved in the `answer` field.      | null                                                                                                                                                                                                                                                         |
| other    | include source or solution. etc..                               | "source": "2017年福建省高考语文试题()"}                                                                                                                                                                                                                                |
