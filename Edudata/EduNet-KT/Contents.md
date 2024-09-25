There are five types of contents that _Santa_ serves to students: _questions_, _lectures_, _payment items_, _coupons_, and _scores_.
# Questions
| Field          | Annotation                                                                                                                                                                                                                                              | Example        |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| question_id    | the ID of the question, which is a form of `q{integer}`                                                                                                                                                                                                 | q2319          |
| bundle_id      | the ID of the bundle containing the question, which is a form of `b{integer}`. Each bundle can contains from 1 to 5 questions.                                                                                                                          | b1707          |
| explanation_id |  ID of corresponding explanations (expert's commentaries) for each bundle, which is a form of `e{integer}`. Note that bundle_ids and explanation_ids are the same for every question                                                                    | e1707          |
| correct_answer | the correct answer of each question recorded as a character between `a` and `d` inclusively. The number of choices depends on the part of the question: every question that does not belong to part 2 has four choices, and part 2 questions have three | a              |
| part           |  the part of each question. It is an integer from **1** to **7**.                                                                                                                                                                                       | 3              |
| tags           | the expert-annotated tags for each question. It is a list of integers, which has a form of `{integer};{integer};...;{integer`                                                                                                                           | 179;53;183;184 |
| deployed_at    | represents the time that each question is started to served in _Santa_, represented as **Unix timestamp in millisecond**                                                                                                                                | 1571279008033  |
# Lectures
Lecture information table contains 5 columns: `lecture_id`, `part`, `tags`, `video_length`, `deployed_at`

| Field        | Annotation                                                                                                                                       | Example       |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------- |
| lecture_id   | the ID of the lecture. It is a form of `l{integer}`                                                                                              | I805          |
| part         | the assigned part of the lecture. It is a single integer from `0` to `7`, where `0` stands for the lecture without any particular part assigned. | 5             |
| tag          | the expert-annotated tag for each lecture, which is a single **integer**. The tags that are used for questions and lectures are the same         | 99            |
| video_length | the running time of the video lecture in **milliseconds**, which is a form of single **integer**                                                 | 230000        |
| deployed_at  | represents the time that each question is started to served in _Santa_, represented as **Unix timestamp in millisecond**                         | 1571279008033 |
Note that some lectures' `tags`, `video_lengths`, and `deployed_at` are not available, and they are recorded as `-1`

# Payment Items
Payment item information table contains 4 columns: `payment_item_id`, `payment_type`, `duration`, and `number_of_questions`.

| Field               | Annotation                                                                                                                                                                                                                                               | Example     |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| payment_item_id     | the ID of the payment. It is a form of `p{integer}`                                                                                                                                                                                                      | P6          |
| payment_type        | he type of the payment, which has two possibilities: `pass` and `paygo`. For `pass`, the student can use _Santa_ for the fixed amount of time (for example, 3 months). For `paygo`, the student can solve fixed number of questions (for example, 4000). | pass        |
| duration            | the amount of time that the student can use _Santa_ when he/she buy a certain `pass`, which is represented in **milliseconds**. When `payment_type` is `paygo`, this is filled up with `-1`                                                              | 15552000000 |
| number_of_questions | the running time of the video lecture in **milliseconds**, which is a form of single **integer**                                                                                                                                                         | -1          |
#  Coupons
Coupon information table consists of 3 columns: `coupon_id`, `coupon_type`, and `duration`

| Field       | Annotation                                                                                                       | Example     |
| ----------- | ---------------------------------------------------------------------------------------------------------------- | ----------- |
| coupon_id   | the ID of the coupon. It is a form of `c{integer}`                                                               | c16         |
| coupon_type | the type of the coupon. It is a form of `type-{integer}`, where the type ID depends on the source of the coupon. | type-1      |
| duration    | duration                                                                                                         | 15552000000 |
