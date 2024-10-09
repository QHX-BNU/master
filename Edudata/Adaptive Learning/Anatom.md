# Download
https://www.fi.muni.cz/adaptivelearning/?a=data

# Information
辨别人体组织器官
The data set is based on the online system [practiceanatomy.com](https://practiceanatomy.com/). The system is available in Czech and English, most users are from Czech Republic (84 %) and Slovakia (11 %). The system uses adaptive algorithms for choosing questions, these algorithms are described in detail in [[1](http://data.practiceanatomy.com/#references)] and [[2](http://data.practiceanatomy.com/#references)].

This data set is static and captures users' interactions from 16 November 2015 to 03 January 2017. The application provides both free and premium content, but interactions with the premium content are excluded from the data set.

The basic statistics of the data set are as follows:

- 18,563 learners;
- 2,894 anatomical items
- 1,182,065 answers

# Description
| Field              | Annotation                                                                                                                      | Example                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- |
| id                 | answer identifier                                                                                                               | 66593                        |
| user               | user's identifier                                                                                                               | 1989                         |
| item_asked         | identifier of the asked item                                                                                                    | 1685                         |
| term_name_asked    | name of the asked item                                                                                                          | posterior belly of digastric |
| item_answered      | identifier of the answered term, empty if the user answered "I don't know"                                                      | 1685                         |
| term_name_answered | name of the answered term                                                                                                       | posterior belly of digastric |
| context_name       | name of the image (context)                                                                                                     | Digastric muscle             |
| type               | type of the answer: (t2d) find the given term on the image; (d2t) pick the name for the highlighted term                        | d2t                          |
| options            | number of options (the asked term included)                                                                                     | 6                            |
| time               | datetime when the answer was inserted to the system                                                                             | 2015-11-17 08:26:35.049357   |
| response_time      | how much time the answer took (measured in milliseconds)                                                                        | 3085                         |
| ip_country         | country retrieved from the user’s IP address                                                                                    | CZ                           |
| ip_id              | meaningless identifier of the user’s IP address                                                                                 | 1431                         |
| lang               | language of the terminology (cs: Czech only, la (cs): Latin with some Czech, en: English only, la (en): Latin with some English |                              |
| locations_asked    | location of the asked term on the human body (JSON)                                                                             | ["Head - Face", "Neck"]      |
| systems_asked      | organ systems of the asked term (JSON)                                                                                          | ["Muscles"]                  |
| locations_answered | locations of the answered term on the human body (JSON)                                                                         | ["Head - Face", "Neck"]      |
| systems_answered   | organ systems of the answered term (JSON)                                                                                       | ["Muscles"]                  |
| practice_filter    | filter used by the user to practice (JSON)                                                                                      | [["category/04"]]            |
