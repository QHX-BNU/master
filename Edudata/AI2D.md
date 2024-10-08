https://www.kaggle.com/datasets/nhtanhnguyn0029/ai2d-zip

# Description
## image
| Field      | Annotation             | Example |
| ---------- | ---------------------- | ------- |
| image_name | Uthe name of the image | 0.png   |


![[Pasted image 20241003204534.png]]

## questions
| Field     | Annotation                                       | Example       |
| --------- | ------------------------------------------------ | ------------- |
| imageName | the name of the image where the question appears | 0.png         |
| questions | the detailed imformation of the problem          | [[AI2D#tip1]] |
### tip1
{
  "What is A in the diagram?": {
    "abcLabel": true,
    "answerTexts": [
      "ears",
      "nose",
      "mouth",
      "face"
    ],
    "correctAnswer": 3,
    "questionId": "0.png-0"
  },
  "What is B in the diagram?": {
    "abcLabel": true,
    "answerTexts": [
      "face",
      "mouth",
      "nose",
      "ears"
    ],
    "correctAnswer": 3,
    "questionId": "0.png-1"
  }
}
## annotations
https://arxiv.org/pdf/1603.07396v1

| Field            | Annotation            | Example |
| ---------------- | --------------------- | ------- |
| imageName        | the name of the image | 0.png   |
| arrowHeads       |                       | 见下图     |
| arrows           |                       |         |
| blobs            |                       |         |
| containers       |                       |         |
| imageConsts      |                       |         |
| meaningfulSpaces |                       |         |
| relationships    |                       |         |
| text             |                       |         |
![[Pasted image 20241003205132.png]]

## categories
| Field     | Annotation                | Example  |
| --------- | ------------------------- | -------- |
| imageName | the name of the image     | 0.png    |
| category  | the category of the image | partsOfA |
