https://github.com/ufal/GECCC

# Description

| Field          | Annotation                                                                                                                                                                                                                                               | Example                           |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| Filename       | ID of the record that is used for linking from the .meta files                                                                                                                                                                                           | tei-skript2012_10-pr1chouluc_01_1 |
| Domain         | one of 4 user domains (_Natives Formal_, _Natives Web Informal_, _Romani_ and _Second Learners_)                                                                                                                                                         | Natives Formal                    |
| Age            | either a 1- or 2-digit string specifying the age of the writer, or 4-digit string indicating writer age range (e.g. 1519 stays for age between 15 and 19) or _Unknown_                                                                                   | 15                                |
| Sex            |  either _F_ (female), _M_ (male) or _Unknown_                                                                                                                                                                                                            | F                                 |
| isSlavic       | either _Yes_ if the writer comes from a Slavic language group, _No_ if he does not or Unknown                                                                                                                                                            | Yes                               |
| Source         | name of the corpus the original noisy document comes from.                                                                                                                                                                                               | Skript2012                        |
| OriginalName   |  ID of the document storing the original sentences regarding the Source. The main purpose of this is to allow linking the GECCC dataset records to their original records that sometimes provide more metadata than Age, Sex and isSlavic that we chose. | pr1chouluc_01_1.xml               |
| NewlyAnnotated | whether the document is annotated with new annotations or the annotation were not newly created and come from the original source                                                                                                                        | No                                |

# Tip1
-The [data](https://github.com/ufal/GECCC/blob/main/data) folder comprises three subfolders: _train_, _dev_ and _test_, each storing files of the particular set. In each folder, eight files can be found:

- _sentence.m2_ – sentences in the M2 format
- _paragraph.m2_ – paragraphs in the M2 format
- _sentence.input_, _sentence.gold_ – aligned detokenized sentences (input with original noisy sentences and gold with one or two of their [alternative] corrections [tab-separated])
- _paragraph.input_, _paragraph.gold_ – aligned detokenized paragraphs (input with original noisy paragraphs and gold with one or two of their [alternative] corrections [tab-separated])
- _sentence.meta_ – each line in this file specifies a pointer to the meta-description file that contains metadata such as the user domain of the sentence writer or the original document the sentence belongs to. Specifically, i-th line of this file stores the pointer for the i-th line of sentence.input and sentence.gold, and i-th record in sentence.m2
- _paragraph.meta_ – same as sentence.meta but for the paragraph-level data. Note that both sentences and paragraphs are in their files in original order and that paragraphs can be joined into documents using information from the paragraph.meta file (all paragraphs belonging to the same document have the same ID).

Note that paragraph-level data contain special character ࿄, which represents the newline. It originates in the fact that while annotating the dataset, annotators were allowed to join two paragraphs into one or split a paragraph into two paragraphs if such change leads to a better text. Also note that we do not include document-level aligned data as they can be easily reconstructed from paragraph-level data and their meta-information.