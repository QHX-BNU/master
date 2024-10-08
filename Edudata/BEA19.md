https://huggingface.co/datasets/juancavallotti/bea-19-corruption
https://www.cl.cam.ac.uk/research/nl/bea2019st/

# Description
| Field     | Annotation               | Example                                                                                                                                                                       |
| --------- | ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id        | the id of the sentence   | 100                                                                                                                                                                           |
| sentence  | the text of the sentence | Consequently , I realized that although ciclyng outside helped me to improve my fitness , really I enjoyed the best breathing fresh air and taking pleasure the countryside . |
| broken    | the corrected sentence   | Consequently , I realized that although ciclyng outside helped me to improve my fitness , really I enjoyed the best breathing pure air and taking pleasure the countryside .  |
| annotator | the id of the annotator  | 0                                                                                                                                                                             |
| tags      | the type of the mistake  | ADJ                                                                                                                                                                           |
| edit      | the M2[[BEA19#tip1]]     | 21 22\|\|\|R:ADJ\|\|\|pure\|\|\|fresh                                                                                                                                         |
# tip1
#### M2 Format

All the above corpora have been made available in M2 format, the standard format for annotated GEC files since the CoNLL-2013 shared task.

S This are a sentence .  
A 1 2|||R:VERB:SVA|||is|||-REQUIRED-|||NONE|||0  
A 3 3|||M:ADJ|||good|||-REQUIRED-|||NONE|||0  
A 1 2|||R:VERB:SVA|||is|||-REQUIRED-|||NONE|||1  
A -1 -1|||noop|||-NONE-|||REQUIRED|||-NONE-|||2

In M2 format, a line preceded by S denotes an original sentence while a line preceded by A indicates an edit annotation. Each edit line consists of the start and end token offset of the edit, the error type, and the tokenized correction string. The next two fields are included for historical reasons and can be ignored (see the CoNLL-2013 shared task), while the last field is the annotator id.

A "noop" edit is a special kind of edit that explicitly indicates an annotator/system made no changes to the original sentence. If there is only one annotator, noop edits are optional, otherwise a noop edit should be included whenever at least 1 out of n annotators considered the original sentence to be correct. This is something to be aware of when combining individual M2 files, as missing noops can affect results.

The above example can hence be interpreted as follows:  
Annotator 0 changed "are" to "is" and inserted "good" before "sentence" to produce the correction: _This is a good sentence ._  
Annotator 1 changed "are" to "is" to produce the correction: _This is a sentence ._  
Annotator 2 thought the original was correct and made no changes to the sentence: _This are a sentence ._