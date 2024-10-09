A major drawback of the question-response sequence format is that it cannot account for the inherent heterogeneity of students' actions. For example, a student may alternately select one of two answer choices before submitting his final answer, which possibly signals that he is unsure of either of the options. Due to the restriction of question-response format, a dataset following such format like EdNet-KT1 can't effectively represent such situation. To overcome this limitation, _Santa_ have collected the full behavior of students since Aug. 27, 2018. As a result, the datasets EdNet-KT2, EdNet-KT3 and EdNet-KT4 of _action sequences_ of each user are compiled. Each _action_ represents a single unit of behavior made by a student in the _Santa_ UI, such as watching a video lecture, choosing a response option, or reading a passage. By recording a student's behavior as-is, the datasets represent each student's behavior more accurately and allows AIEd models to incorporate finer details of learning history. EdNet-KT2, the simplest action-based dataset of EdNet, consists of the actions related to question-solving activities. Note that the features of KT1 can be fully recovered by the columns of KT2, and KT2 contains further information such as the study mode of student or the intermediate responses provided by student.

# Description
One csv file is One student, like "u717875.csv"

| Field       | Annotation                                                                                                                                                    | Example       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| action_type |  [tip1](#tip1)                                                                                                                                            | enter         |
| item_id     |  [tip2](#tip2)                                                                                                                                           | b4957         |
| source      |  [tip3](#tip3)                                                                                                                                            | diagnosis     |
| user_answer | `user_answer` is recorded when `action_type` is `respond`, which stands for the student's submitted answer. It is one of the alphabets `a`, `b`, `c`, and `d` | a             |
| platform    | `platform` shows where the student used _Santa_, which is either **mobile** or **web**.                                                                       | mobile        |
| timestamp   | the moment the question was given, represented as **Unix timestamp in milliseconds**.                                                                         | 1358114668713 |
## tip1
- `action_type` is one of the following: `enter`, `respond`, and `submit`.
    
    - `enter` is recorded when student first receives and views a question bundle through UI.
    - `respond` is recorded when the student selects an answer choice to one of the questions in the bundle. A student can respond to the same question multiple times. In this case, only the last response before submitting his final answer is considered as his response.
    - `submit` is recorded when the student submits his final answers to the the given bundle.
## tip2
The ID of item involved with the action. For EdNet-KT2, only the IDs of questions and bundles are recorded. A bundle is assigned for actions of type `enter` and `submit`.
## tip3
- `source` shows _where_ the student solve a question or watch a lecture in _Santa_ UI. There are several sources in _Santa_ that students can solve questions or watch lectures. For KT2, only the sources that provides question-solving environments are recorded.
    
    - In `sprint`, students choose a part that they want to study. After that, they can only solve questions belongs to the part that they choose, until they change to different part or select different source.
        
    - For each day, _Santa_ recommends questions and lectures based on each student's current knowledge status, i.e. correctness probabilities predicted by the Collaborative Filtering model. Such source is called _Today's Recommendation_. Questions that belong to particular parts can be recommended, `todays_recommendation::sprint`, `todays_recommendation::review_quiz`
        
    - Once the number of incorrect answers to questions with particular tags exceeds certain threshold, _Santa_ suggests lectures and questions with corresponding tags. Such suggestion is recorded as `adaptive_offer`. It also offers lectures and questions if the average correctness rate of questions with particular tags decreased by more than a certain threshold.
        
    - _All Parts_ is a source that students solve questions that _Santa_ recommends following a certain algorithm, from all possible candidates. This is recorded as `tutor`.
        
    - The student can re-do the questions that he already solved before using _review_ system, which is recorded as `in_review`.
