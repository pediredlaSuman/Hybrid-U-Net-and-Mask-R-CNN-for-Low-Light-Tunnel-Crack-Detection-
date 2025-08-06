<img width="546" height="358" alt="image" src="https://github.com/user-attachments/assets/a6925f04-7039-43cd-8729-d64dafe0a9fe" />U-Net and mask RCNN model to segment/cemetery tunnel cracks, even in the challenging conditions
– It achieves high accuracy (IoU: 0.847, Dice: 0.918), and it successfully detects the hairline, transverse, longitudinal,
and disguised cracks in the KICT Tunnel Crack Segmentation dataset.

Develop a Deep Learning-Based Crack Detection System

Preprocess and Augment the Dataset for Better Generalization

Train and Fine-Tune the Segmentation Model

Visualize Model Predictions for Crack Detection

Save and Deploy the Model for Future Use

<img width="776" height="601" alt="image" src="https://github.com/user-attachments/assets/70d85f88-95b0-48dc-bd72-ac4caa48de5a" />

🔹U-Net segments low-light tunnel
images to generate initial crack masks.
                                                     <img width="546" height="358" alt="image" src="https://github.com/user-attachments/assets/68d5ba4a-0c28-4916-baa9-770f382fe2ad" />
🔹These masks highlight crack regions for
refinement.
🔹Mask R-CNN uses the image and mask               <img width="798" height="294" alt="image" src="https://github.com/user-attachments/assets/f964c49d-d0f3-49f9-a924-9e2212837914" />

to detect and classify cracks accurately.
🔹 The hybrid model enhances crack
detection in complex tunnel scenes.
🔹Combines pixel-wise segmentation with
instance-level detection for robust crack
localization


