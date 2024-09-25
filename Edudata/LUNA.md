https://base.ustc.edu.cn/data/OpenLUNA/
# Description
| Field         | Annotation        | Example                       |
| ------------- | ----------------- | ----------------------------- |
| stem（str）     | 试题题干              | 若复数$z=1+2 i+i^{3}$，则$\|z\|=$  |
| options(list) | 试题选项              | ['0', '1', '$\sqrt{2}$', '2'] |
| type（int）     | 试题类型[[LUNA#Tip1]] | 6                             |
# Tip1
* 0 混合类型以及其他类型  
* 1 多选题  
* 2 填空题  
* 3 判断题  
* 4 简答题  
* 5 计算题  
* 6 单选题

简单的问题文本