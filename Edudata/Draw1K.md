https://www.microsoft.com/en-us/download/details.aspx?id=52628
# Description
| Field      | Annotation                                                                                  | Example                                                                                                                                                             |
| ---------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| sQuestion  | the content of the questions                                                                | In a chemistry class , 5 liters of 4 % silver solution must be mixed with a 10 % solution to get a 6 % solution . How many liters of the 10 % solution are needed ? |
| lEquations | the equation of the problem                                                                 | 01*4*(5)+.01*10*x=.01*6*(5+x)                                                                                                                                       |
| ISolutions | the answer of the question                                                                  | 2.5                                                                                                                                                                 |
| Template   | the template; a, b, ... represents the coefficients while m,n, ... represents the variables | a * m - b * m = b * c - c * d                                                                                                                                       |
| iIndex     | problem id                                                                                  | 300319                                                                                                                                                              |
| Alignment  | the alignments between the coefficients and textual numbers a json file                     | [[Draw1K#Tip1]]                                                                                                                                                     |
 

# Tip1
coeff:template中的系数
sentenceID: 系数在问题中的句子的ID
value:系数的值
TokenID: 系数的tokenID
 {
    "coeff": "d", 
    "SentenceId": 0, 
    "Value": 4.0, 
    "TokenId": 8
   }, 
   {
    "coeff": "c", 
    "SentenceId": 0, 
    "Value": 5.0, 
    "TokenId": 5
   }, 
   {
    "coeff": "a", 
    "SentenceId": 0, 
    "Value": 10.0, 
    "TokenId": 17
   }, 
   {
    "coeff": "b", 
    "SentenceId": 0, 
    "Value": 6.0, 
    "TokenId": 23
   }