# Download
https://crfm.stanford.edu/helm/lite/v1.9.0/
https://huggingface.co/datasets/deepmind/narrativeqa

# Description
| Field                   | Annotation                                                                     | Example                                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| document.id             | Unique ID for the story                                                        | 23jncj2n3534563110                                                                                            |
| document.kind           | "movie" or "gutenberg" depending on the source of the story.                   | gutenberg                                                                                                     |
| document.url            | The URL where the story was downloaded from.                                   | http://www.gutenberg.org/(...TRUNCATED)                                                                       |
| document.file_size      | File size (in bytes) of the story.                                             | 80473<br>                                                                                                     |
| document.word_count     | Number of tokens in the story.                                                 | 4100                                                                                                          |
| document.start          | irst 3 tokens of the story. Used for verifying the story hasn't been modified. | <br>MOVIE screenplay by                                                                                       |
| document.end            | Last 3 tokens of the story. Used for verifying the story hasn't been modified. | . THE END                                                                                                     |
| document.summary.text   | Text of the wikipedia summary of the story.                                    | <br>Joe Bloggs begins his journey exploring...                                                                |
| document.summary.tokens | Tokenized version of `document.summary.text`.                                  | <br> ["Joe", "Bloggs", "begins", "his", "journey", "exploring",...]<br>                                       |
| document.summary.url    | Wikipedia URL of the summary.                                                  | <br>http://en.wikipedia.org/wiki/Name_of_Movie                                                                |
| document.summary.title  | Wikipedia Title of the summary.                                                | Name of Movie (film)<br>                                                                                      |
| question                | `{"text":"...", "tokens":[...]}` for the question about the story.             | <br>"text": "Where does Joe Bloggs live?",<br> "tokens": ["Where", "does", "Joe", "Bloggs", "live", "?"],     |
| answers                 | List of `{"text":"...", "tokens":[...]}` for valid answers for the question.   | <br> {"text": "At home", "tokens": ["At", "home"]},<br> {"text": "His house", "tokens": ["His", "house"]}<br> |