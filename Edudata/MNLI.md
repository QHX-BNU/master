# Download
https://huggingface.co/datasets/nyu-mll/multi_nli

# Description
| Field                   | Annotation                                                                                                   | Example                                                                                                                                                                        |
| ----------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| promptID                | Unique identifier for prompt                                                                                 | 31193                                                                                                                                                                          |
| pairID                  | Unique identifier for pair                                                                                   | 31193n<br>                                                                                                                                                                     |
| premise                 | the text of the premise                                                                                      | Conceptually cream skimming has two basic dimensions - product and geography.                                                                                                  |
| premise parse           | Each sentence as parsed by the Stanford PCFG Parser 3.5.2                                                    | (ROOT (S (NP (JJ Conceptually) (NN cream) (NN skimming)) (VP (VBZ has) (NP (NP (CD two) (JJ basic) (NNS dimensions)) (: -) (NP (NN product) (CC and) (NN geography)))) (. .))) |
| premise binary parse    | parses in unlabeled binary-branching format                                                                  | ( ( Conceptually ( cream skimming ) ) ( ( has ( ( ( two ( basic dimensions ) ) - ) ( ( product and ) geography ) ) ) . ) )                                                     |
| hypothesis              | the text of the hypothesis                                                                                   | Product and geography are what make cream skimming work.                                                                                                                       |
| hypothesis_parse        | Each sentence as parsed by the Stanford PCFG Parser 3.5.2                                                    | (ROOT (S (NP (NN Product) (CC and) (NN geography)) (VP (VBP are) (SBAR (WHNP (WP what)) (S (VP (VBP make) (NP (NP (NN cream)) (VP (VBG skimming) (NP (NN work)))))))) (. .)))  |
| hypothesis_binary_parse | parses in unlabeled binary-branching format                                                                  | ( ( ( Product and ) geography ) ( ( are ( what ( make ( cream ( skimming work ) ) ) ) ) . ) )                                                                                  |
| genre                   | the genre of the sentence                                                                                    | government                                                                                                                                                                     |
| label                   | a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2). | 1                                                                                                                                                                              |