U-Net and mask RCNN model to segment/cemetery tunnel cracks, even in the challenging conditions
It achieves high accuracy (IoU: 0.847, Dice: 0.918), and it successfully detects the hairline, transverse, longitudinal,
and disguised cracks in the KICT Tunnel Crack Segmentation dataset.

Developed a Deep Learning-Based Crack Detection System. Preprocessed and Augmented the Dataset for Better Generalization.Train and Fine-Tune the Segmentation Model. Visualized Model Predictions for Crack Detection. Saved and Deployed the Model for Future Use

<img width="776" height="601" alt="image" src="https://github.com/user-attachments/assets/70d85f88-95b0-48dc-bd72-ac4caa48de5a" />

🔹U-Net segments low-light tunnel                   <img width="546" height="358" alt="image" src="https://github.com/user-attachments/assets/68d5ba4a-0c28-4916-baa9-770f382fe2ad" />
images to generate initial crack masks.
🔹These masks highlight crack regions for
refinement.
🔹Mask R-CNN uses the image and mask               <img width="798" height="294" alt="image" src="https://github.com/user-attachments/assets/f964c49d-d0f3-49f9-a924-9e2212837914" />
to detect and classify cracks accurately.
🔹 The hybrid model enhances crack
detection in complex tunnel scenes.
🔹Combines pixel-wise segmentation with
instance-level detection for robust crack
localization

Experimental results and discussion:

<img width="685" height="328" alt="image" src="https://github.com/user-attachments/assets/b2b80903-efcc-4476-8df6-88377e1914dd" /><img width="702" height="308" alt="image" src="https://github.com/user-attachments/assets/ab4f76c6-0337-4784-af97-8d8b9206d4a7" /><img width="667" height="337" alt="image" src="https://github.com/user-attachments/assets/90a934fe-c589-43c4-a207-7c2b49f2b674" /><img width="740" height="336" alt="image" src="https://github.com/user-attachments/assets/a2cbde22-ad46-49fb-a646-2d4542cd5a45" /><img width="702" height="348" alt="image" src="https://github.com/user-attachments/assets/f6cf1b1f-94f3-4f32-a7d3-8b66e85521a7" /><img width="884" height="280" alt="image" src="https://github.com/user-attachments/assets/143a3112-677e-4596-a1af-7981f5f28eda" /><img width="920" height="297" alt="image" src="https://github.com/user-attachments/assets/24fa2756-2775-43e4-8493-aab9fb75fb46" /><img width="874" height="275" alt="image" src="https://github.com/user-attachments/assets/30f4d3e6-c24a-4f01-b125-c60d416f22dc" />



