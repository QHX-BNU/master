In EdNet-KT4, a complete list of actions collected by _Santa_ is provided. In particular, the following types of actions are added to EdNet-KT3: `erase_choice`, `undo_erase_choice`, `play_audio`, `pause_audio`, `play_video`, `pause_video`, `pay`, `refund`, and `enroll_coupon`.

# Description
| Field       | Annotation                                                                                                                                                    | Example       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| action_type | reference to ```EdNet-KT2 tip1``` besides 'quit' and [tip1](#tip1)                                                                                                           | enter         |
| item_id     | reference to ```EdNet-KT2#tip2```                                                                                                                                            | b4957         |
| source      | reference to ```EdNet-KT2#tip3```                                                                                                                                            | diagnosis     |
| user_answer | `user_answer` is recorded when `action_type` is `respond`, which stands for the student's submitted answer. It is one of the alphabets `a`, `b`, `c`, and `d` | a             |
| platform    | `platform` shows where the student used _Santa_, which is either **mobile** or **web**.                                                                       | mobile        |
| timestamp   | the moment the question was given, represented as **Unix timestamp in milliseconds**.                                                                         | 1358114668713 |
| cursor_time |                                                                                                                                                               | 10000         |
## tip1
- `erase_choice`, `undo_erase_choice`
    - For user's convenience, a student can hide an answer choice by erasing it. He can also undo his action to consider the choice again. The act of erasing a choice and undoing it are given as actions of type `erase_choice` and `undo_erase_choice` respectively. The answer choice erased/un-erased is supplied in the `user_answer` column.
- `play_audio`, `pause_audio`, `play_video`, `pause_video`
    - A student can play or pause a given multimedia asset. For videos, he can also navigate to different moments of the video by moving his cursor to different places. Such actions are denoted as one of the action types `play_audio`, `pause_audio`, `play_video` or `pause_video`. A column `cursor_time` is added to EdNet-KT4, to represent the moment where he has played or paused the media.
- `pay`, `refund`
    - By default, a free user is offered 10 questions of Part 2 and 5 each daily. By purchasing a payment item, the student have full access to questions of all parts. A table of payment items is provided separately (see below). Items of type `pass` allows solving all questions for the time `duration` in milliseconds. Items of type `paygo` allows student to solve the specific number of bundles denoted by column `number_of_bundles`.
- `enroll_coupon`
    - A student may enter his promotion coupon code to receive corresponding benefits. The ID of his coupon and the time he entered the coupon is recorded as an action of type `enroll_coupon`. A table of coupons is provided separately (see below).

