https://huggingface.co/datasets/matejklemen/clc_fce

# Description
| Field          | Annotation                        | Example                                                                                                                                                         |
| -------------- | --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| src_tokens<br> | the tokens of the source sentence | [ "I", "am", "writing", "in", "order", "to", "express", "my", "disappointment", "about", "your", "musical", "show", "\"", "Over", "the", "Rainbow", "\"", "." ] |
| tgt_tokens     | the tokens of the target sentence | [ "I", "am", "writing", "in", "order", "to", "express", "my", "disappointment", "with", "your", "musical", "show", "\"", "Over", "the", "Rainbow", "\"", "." ]  |
| corrections    | the correction of the sentence    | [ { "idx_src": [ 9 ], "idx_tgt": [ 9 ], "corr_type": "R:PREP" } ]                                                                                               |