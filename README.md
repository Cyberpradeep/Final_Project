# Garbage Classification with MobileNetV2 (Transfer Learning)

**Author**: Cyberpradeep  
**Repo**: [Final_Project](https://github.com/Cyberpradeep/Final_Project)  
**Model**: Trained on 6 garbage types using MobileNetV2  
**Interface**: Gradio Web UI

---

## Objective

Build a deep learning model that can classify images of garbage into categories like:
- `cardboard`
- `glass`
- `metal`
- `paper`
- `plastic`
- `trash`

This promotes smart waste segregation, essential for environmental sustainability 🌍♻️.

---

## Project Highlights

-  **Transfer Learning** with MobileNetV2 (`imagenet` weights)
- Trained with images organized into 6 class folders
- 224x224 image input, normalized and augmented
- Final `.h5` model saved in Google Drive
- Deployed with **Gradio** for real-time predictions

---

---

## Model Architecture

-  Base model: **MobileNetV2** (frozen during initial training)
-  Custom classifier head:
  - GlobalAveragePooling2D  
  - BatchNormalization  
  - Dense(128, relu) + Dropout  
  - Dense(10, softmax)
-  Optimizer: Adam
-  Loss: sparse_categorical_crossentropy

---


## Accuracy

![Screenshot 2025-07-03 115434](https://github.com/user-attachments/assets/9d00aff0-b092-4ff2-a8ed-b7e3b3979f2e)

![Screenshot 2025-07-03 115836](https://github.com/user-attachments/assets/a35cd832-4a9f-4f94-bd98-df01f441ec5d)


## Output Screenshots

![Screenshot 2025-07-03 114806](https://github.com/user-attachments/assets/7ab2ee52-0b17-4f27-a305-b67c65648a38)
![Screenshot 2025-07-03 115828](https://github.com/user-attachments/assets/726f737a-4cd3-4672-b0ed-567a89db6fa5)

