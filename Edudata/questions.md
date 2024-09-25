# ASSITMENT2017
## 1 
Avgcarelessness 考虑Slip和Guess,这是原始的文章
Baker, R.S.J.d., Corbett, A.T., Aleven, V.: Improving Contextual Models of Guessing and Slipping with a Truncated Training Set. In: Proceedings of the 1st International Conference on Educational Data Mining, pp. 67–76 (2008)
在这篇文章中，
![[Pasted image 20240913190835.png]]
在上图中，为什么在掌握知识的情况下错误的概率是P(G)而不是P(S),G表示‘guess’,S表示‘Slip’

# 2
什么是 bottom-out hint?? 我的理解是最全面的提示
# 3
skill字段，有几种类型？？是否表示布鲁姆知识的水平：知道，应用，分析，综合，创新
![[Pasted image 20240914113909.png]]
# 4
有些字段的描述是NaN，比如“prev5count”。我看官网上对于该字段的描述也不清楚，这些字段的具体含义是什么？是否可以忽略？？
# 5
| Enrolled  |     |
| --------- | --- |
| Selective |     |
| isSTEM    |     |
这三个字段在标签说明中没有，我看了原始数据集中也没有，为什么在EduData上存在，具体代表什么意思？？
# 6
first_response表示什么意思？刚开始我认为是解决问题的第一个反应或者操作，但是后来看到最后五个包含请求的first response？？我的理解是第一反应，为什么有这么多“第一反应”？？
# EdNet
EduData上没有KT2，KT3，KT4的描述，
勘误：有的，不过实在gitHub上，不在EduData网站上
其中KT4中有一个字段cursor_time表示什么意思？？麻烦师姐可以可以看看
# Math2015
是不是2015年高考的数学试卷？？
# OLI fall 2011
## problem
#### 1 
Correct First Attempts ：Total number of correct first attempts made by the student for this problem
为什么第一次尝试还有数量？？第一次不应该就是一次吗？
### 2
Steps without KCs：Total number of steps in this problem (performed by the student) without an assigned KC.
这个字段和Steps有什么区别？？什么是没有指定KC的步骤？？

### 3
| KCs (Single-KC)                 |
| ------------------------------- |
| Steps without KCs (Single-KC)   |
| KC List (Single-KC)             |
| KCs (Unique-step)               |
| Steps without KCs (Unique-step) |
| KC List (Unique-step)           |
这几个字段是什么意思？？我再Datashop上好像没有找到这个数据集？？OLI具体代表什么数据集？？
## step
### 1
Step Start Time:2011/9/21 17:35
Step End Time:2011/9/21 17:35
Step Duration (sec):23.13
Duration不应该是0吗？这是我在EduData看到的sample??
### 2
| KC (Unique-step)[[Step#tip3]]      |
| ---------------------------------- |
| Opportunity (Unique-step)          |
| Predicted Error Rate (Unique-step) |
这几个字段是什么意思？？

## tranction
### 1
| Level (level_type)[[Transaction#tip1]] | The problem hierarchy name (e.g., "Understanding Fractions") of the type specified in the column header (e.g., "Unit"). There may be multiple "Level" columns if the problem hierarchy is more than one level deep. Level is logged in the level element.                                                                                                                                                                                                                                                                                                                                                                               | Level(Squence) Statics<br>Level(Unit) Concentrated Forces and Their Effects<br>Level(Module)  Introduction to Free Body Diagrams<br>Level(Section1) NaN |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
Level (level_type) 是什么意思？？
水平有高下之分吗？？只看字段好像看不出来？？

### 2
数据集的标签描述和sample的数据字段不一致？？
https://edudata.readthedocs.io/en/latest/build/blitz/OLI_Fall2011/OLI_2011F_transaction.html
