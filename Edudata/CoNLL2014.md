https://www.comp.nus.edu.sg/~nlp/conll14st.html

[Grammatical Error Correction](https://www.comp.nus.edu.sg/~nlp/conll14st/CoNLLST01.pdf)

# Description
[[CoNLL2014#Example]]

| Field      | Annotation                                      | Example                                                             |
| ---------- | ----------------------------------------------- | ------------------------------------------------------------------- |
| nid        | the id of the paasage                           | 1                                                                   |
| annotation | the id of the teacher who corrected the passage | 42                                                                  |
| mistake    | the mitake of the passage                       | start_par="2" <br>start_off="144" <br>end_par="2" <br>end_off="148" |
| type       | the type of the mistake                         | Vm                                                                  |
| correction | the correction of the mistake                   | have go                                                             |
ERROR TAG    ERROR CATEGORY
---------------------------
Vt	     Verb tense
Vm	     Verb modal
V0	     Missing verb
Vform	     Verb form
SVA	     Subject-verb-agreement
ArtOrDet     Article or Determiner
Nn	     Noun number
Npos	     Noun possesive
Pform	     Pronoun form
Pref	     Pronoun reference
Prep         Preposition
Wci	     Wrong collocation/idiom
Wa	     Acronyms
Wform	     Word form
Wtone	     Tone
Srun	     Runons, comma splice
Smod	     Dangling modifier
Spar	     Parallelism
Sfrag	     Fragment
Ssub	     Subordinate clause
WOinc	     Incorrect sentence form
WOadv	     Adverb/adjective position
Trans	     Link word/phrases
Mec	     Punctuation, capitalization, spelling, typos
Rloc-	     Local redundancy
Cit	     Citation
Others	     Other errors
Um	     Unclear meaning (cannot be corrected)

# tip1
The corpus is distributed in a simple SGML format.  All annotations
come in a "stand-off" format. The start position and end position of
an annotation are given by paragraph and character offsets.
Paragraphs are enclosed in \<P>...\</P> tags. Paragraphs and characters
are counted starting from zero. Each annotation includes the following
fields: the error category, the correction, and optionally a
comment. If the correction replaces the original text at the given
location, it should fix the grammatical error.

# Example
<DOC nid="1">
<ANNOTATION teacher_id="42">
<MISTAKE start_par="2" start_off="144" end_par="2" end_off="148">
<TYPE>Vm</TYPE>
<CORRECTION>have got</CORRECTION>
</MISTAKE>
<MISTAKE start_par="2" start_off="148" end_par="2" end_off="155">
<TYPE>ArtOrDet</TYPE>
<CORRECTION>a certain</CORRECTION>
</MISTAKE>
<MISTAKE start_par="2" start_off="171" end_par="2" end_off="180">
<TYPE>Mec</TYPE>
<CORRECTION>attitudes</CORRECTION>
</MISTAKE>
<MISTAKE start_par="2" start_off="186" end_par="2" end_off="203">
<TYPE>Vform</TYPE>
<CORRECTION>easily change</CORRECTION>
</MISTAKE>
<MISTAKE start_par="2" start_off="205" end_par="2" end_off="212">
<TYPE>Others</TYPE>
<CORRECTION>whether it be</CORRECTION>
<COMMENT>subj and verb added</COMMENT>
</MISTAKE>
<MISTAKE start_par="2" start_off="213" end_par="2" end_off="219">
<TYPE>Prep</TYPE>
<CORRECTION>caring about</CORRECTION>
</MISTAKE>
<MISTAKE start_par="5" start_off="39" end_par="5" end_off="46">
<TYPE>ArtOrDet</TYPE>
<CORRECTION>a certain</CORRECTION>
</MISTAKE>
<MISTAKE start_par="5" start_off="47" end_par="5" end_off="54">
<TYPE>Rloc-</TYPE>
<CORRECTION></CORRECTION>
</MISTAKE>
<MISTAKE start_par="5" start_off="142" end_par="5" end_off="148">
<TYPE>Spar</TYPE>
<CORRECTION>to make it known</CORRECTION>
</MISTAKE>
<MISTAKE start_par="5" start_off="148" end_par="5" end_off="150">
<TYPE>Prep</TYPE>
<CORRECTION>to</CORRECTION>
</MISTAKE>
</ANNOTATION>
</DOC