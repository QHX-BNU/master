# More information
https://github.com/arozovskaya/RULEC-GEC
If you are interested in more information about the dataset, please apply in the link above.

# Description
| Field      | Annotation                                                                                                                                                                                                                                                                                              | Example |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| id         | the id of the sentence.  The sentence ID includes the name of the annotator, followed by the name of the original file in RULEC, followed by the sentence number, as it appears in the essay. The sentence ID ends with the square bracket symbol ([) and is followed by the tokenized sentence itself. |         |
| sentence   | the text of the sentence                                                                                                                                                                                                                                                                                |         |
| M2         | the M2 formation of the sentence                                                                                                                                                                                                                                                          |         |
# Tip1
_startTokenID_ corresponds to the first token in the annotation (sentence-initial token has ID of 0) _endTokenID_ corresponds to the token that immediately follows the last token included in the correction _ErrorType_ -- specifies the type of error (error types are listed below) _Corrected form_ -- can be empty string (if a deletion); otherwise contains one or multiple tokens that should be used to replace the original tokens specified with the startTokenID and endTokenID

# Error Type
```
Орфография Spelling
Сущ.:Падеж Noun:case
Лексика:замена Lexical choice
Пунктуация Punctuation (punc. errors are marked as Delete or Insert in the M2 files)
Вставить Insert
Заменить Replace
Убрать Delete
Прил.:Падеж Adj:Case
Предлог Preposition
Лексика:морф.  Word form
Сущ.:Число Noun:Number
Глагол:Число/Лицо Verb:Number/Person
Глагол:Вид Verb:Aspect
Прил.:Род Adj:Gender
Глагол:Залог Verb:Voice
Глагол:Время Verb:Tense
Прил.:Др. Adj:Other
Местоимение Pronoun
Прил.:Число Adj:Number
Союз Conjunction
Глагол:Др. Verb:Other
Сущ.:Род Noun:Gender
Сущ.:Др. Noun:Other
```
