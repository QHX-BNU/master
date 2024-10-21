# Download
https://amritasaha1812.github.io/CSQA/

# Paper
**Complex sequential question answering: To wards learning to converse over linked question an swer pairs with a knowledge graph**

# Description
| Field                 | Annotation                                                               | Example      |
| --------------------- | ------------------------------------------------------------------------ | ------------ |
| ques_type_id          | ID corresponding to the question utterance                               |              |
| description           | Description of type of question                                          |              |
| relations             | ID's of predicates used in the utterance                                 | <br><br><br> |
| entities_in_utterance | ID's of entities used in the question                                    |              |
| speaker               | The nature of speaker: SYSTEM or USER                                    |              |
| utterance             | The utterance: either the question, clarification or response            |              |
| active_set            | A regular expression which identifies the entity set of answer list      |              |
| all_entities          | List of ALL entities which constitute the answer of the question         |              |
| question-type         | ype of question (broad types used for evaluation as in Table-4 of paper) |              |
| type_list             | List containing entity IDs of all entity parents used in the question    |              |
# Example
|                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------- |
| **USER:** Which people were casted in The 36th Chamber of Shaolin ?                                                                                |
| **SPEAKER:** Gordon Liu, Lo Lieh                                                                                                                   |
| **USER:** Which works of art stars Gordon Liu and Lo Lieh as actor ?                                                                               |
| **SPEAKER:** Kill Bill Volume 1, Flying Swords of Dragon Gate, The Man with the Iron Fists                                                         |
| **USER:** Which language was used originally for the creation of that work of art ?                                                                |
| **SPEAKER:** Did you mean Kill Bill Volume 1 ?                                                                                                     |
| **USER:** No, I meant The Man with the Iron Fists. Could you tell me the answer for that?                                                          |
| **SPEAKER:** English                                                                                                                               |
| **USER:** How many notations are used as the scripts for approximately the same number of languages as Coptic alphabet ?                           |
| **SPEAKER:** 4                                                                                                                                     |
| **USER:** And what about Bamum script?                                                                                                             |
| **SPEAKER:** 4                                                                                                                                     |
| **USER:** Which languages are English or Latin script the writing system of ?                                                                      |
| **SPEAKER:** The answer count is 33. Do you want to see all possibilities?                                                                         |
| **USER:** No, show only a few of them                                                                                                              |
| **SPEAKER:** Norn, Wailaki language, Slavoserbian, Polabian, Sierra Puebla Nahuatl, Basque, Gaulish, Central Nahuatl, Pangasinan language, Nynorsk |
| **USER:** Which languages have writing system as English and Latin script ?                                                                        |
| **SPEAKER:** Pangasinan language, Wailaki language, Gaulish, Norn, Central Nahuatl, Slavoserbian, Basque, Sierra Puebla Nahuatl, Polabian, Nynorsk |
| **USER:** How many notations are the writing systems used for approximately 1 language ?                                                           |
| **SPEAKER:** 4                                                                                                                                     |
| **USER:** How many classification schemes are English a component of ?                                                                             |
| **SPEAKER:** 2                                                                                                                                     |
| **USER:** And also tell me about German submarine U-42?                                                                                            |
| **SPEAKER:** 1                                                                                                                                     |