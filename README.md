# DS4-Final-Project

This project demonstrates the full object detection pipeline using RF-DETR, a transformer-based architecture developed by Roboflow. The goal is to detect and classify animals in images using a custom COCO-formatted dataset sourced from Roboflow Universe.

We trained the model for 15 epochs on a dataset of 1700 images, using gradient accumulation and data augmentation (±15° rotation, normalization). The training process was handled via the rfdetr Python package, and performance was monitored through loss curves and precision-recall plots.

After training, the model was evaluated on the test set. Visual comparisons were made between predicted and ground truth bounding boxes using the Supervision library. Key metrics such as mean Average Precision (mAP), accuracy, precision, recall, and F1-score were computed to assess performance. A confusion matrix was also generated for class-wise evaluation.

Despite the dataset's modest size, the model achieved:

Accuracy: 80.88%

Precision (macro): 83.08%

Recall (macro): 76.76%

F1 Score (macro): 79.44%

These results suggest solid generalization and highlight RF-DETR’s effectiveness in detecting diverse animal classes, though some misclassifications occurred in visually similar categories.

Members:
Maria Alessandra Capili

Darla Zoleta

References: 

Roboflow. (n.d.). RT-DETR: Real-time object detection with transformers. https://roboflow.com/model/rt-detr

Johnson, J. (2023, July 27). How to train RT-DETR on a custom dataset with transformers. Roboflow. https://blog.roboflow.com/train-rt-detr-custom-dataset-transformers/

Murtaza, S. (2024, January 15). RF-DETR: An open-source object detection model. LearnOpenCV. https://learnopencv.com/rf-detr-object-detection/

Sharma, A. (2025, March). Roboflow’s RF-DETR: A powerful object detection model. Analytics Vidhya. https://www.analyticsvidhya.com/blog/2025/03/roboflows-rf-detr/

Tang, Y., Li, Z., Wu, L., He, Y., Huang, G., & Wang, X. (2025). RT-DETR: RT-DETR: Real-Time Detection Transformer (arXiv preprint arXiv:2504.13099v1). https://arxiv.org/abs/2504.13099v1
