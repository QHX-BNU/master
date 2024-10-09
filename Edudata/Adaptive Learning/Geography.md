# Download
https://www.fi.muni.cz/adaptivelearning/?a=data
# Description
## Geography
. A supplementary file describes the used geographical items (file place.csv with columns: ID, code, name of place, type of place, list of maps on which the place occurs, file place_type.csv with description of types of places).
### Answer

| Field          | Annotation                                                                                                                                      | Example             |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
| id             | Answer identifier [Tip1](#Tip1)                                                                                                             | 2407                |
| user           | User’s identifier                                                                                                                               | 75                  |
| place_asked    | Identifier of the asked place                                                                                                                   | 130                 |
| place_answered | Identifier of the answered place; empty if the user answered “I do not know”                                                                    | 69                  |
| type           | Type of question: 1) find the given place on the map; 2) pick the name for the highlighted place                                                | 1                   |
| options        | List of identifiers of options (including the asked place)                                                                                      | [58, 219, 69, 130]  |
| inserted       | Time (yyyy-mm-dd hh:mm:ss) when the answer was inserted in the system                                                                           | 2013-09-26 14:46:03 |
| response_time  | Time spent by the user in answering (measured in milliseconds)                                                                                  | 8526                |
| place_map      | Identifier of the map used in the question (e.g., a question about France may be asked in the context of the map of Europe or the map of world) | NaN                 |
| ip_country     | Country retrieved from the user’s IP address                                                                                                    |                     |
| ip_id          | Meaningless identifier of the user’s IP address                                                                                                 |                     |
| language       | Language version of the system: 0) Czech, 1) English, 2) Spanish                                                                                | 0                   |
### Place
| Field | Annotation                                                  | Example |
| ----- | ----------------------------------------------------------- | ------- |
| id    | Place identifier                                            | 1       |
| code  | Place code                                                  | us-al   |
| name  | IPlace name                                                 | Alabama |
| type  | type of [place](#Place type) | 7       |
| maps  | list of maps on which the place occurs,                     | [195]   |
### [Place type](#Tip2)
| Field | Annotation             | Example |
| ----- | ---------------------- | ------- |
| id    | identifier of the type | 1       |
| name  | name of the type       | country |

# Tip1
One user have one or more answers
# Tip2
1;country  
2;city  
3;world  
4;continent  
5;river  
6;lake  
7;region  
8;mountains  
9;island
