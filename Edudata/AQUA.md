# Download
https://datasets.activeloop.ai/docs/ml/datasets/aqua-dataset/

# Description
| Field                   | Annotation                                                      | Example                                 |
| ----------------------- | --------------------------------------------------------------- | --------------------------------------- |
| index                   | the id of the question                                          | 0                                       |
| image                   | tensor containing the face image                                | ![Pasted image 20241009153741](https://github.com/user-attachments/assets/bf14ff81-80ed-42de-95da-89fe4a9009b0)|
| need_external_knowledge | a binary tensor of True/False                                   | 1                                       |
| questions               | a text tensor containing questions related to the image         | what do a statue of a man stand next to |
| answers                 | a text tensor containing answers related to the question asked. | painting                                |