# Methodology

## Objective

The objective of the study was to develop a CNN-based predictive model that can identify the conclusion of Gallbladder Dissection Phase 4 during laparoscopic cholecystectomy procedures. This prediction supports dynamic operating room schedule updates.

## Data source

The dataset consisted of laparoscopic surgery videos. The study used:

- 20 laparoscopic video recordings obtained during procedures at Al-Salt Hospital in Jordan
- The Cholec80 dataset
- A total of 100 videos

Ten videos were reserved for testing. The remaining videos were used to extract frames for model training and validation.

## Data preparation

The data preparation process included:

1. **Frame extraction**  
   Laparoscopic videos were discretized into individual frames using Python OpenCV.

2. **Central cropping**  
   The central part of each frame was cropped to focus the model on the visual area most relevant to detecting the end of Phase 4.

3. **Binary labeling**  
   Frames were labeled for supervised learning. The classification task focused on whether the frame indicates the termination of Gallbladder Dissection Phase 4.

4. **Data augmentation**  
   The original 240 extracted frames were augmented to generate 960 frames. Augmentation was used to increase training diversity and improve model robustness.

## Train-validation-test structure

The study used:

- 80% of the augmented frame data for training
- 20% of the frame data for validation
- 10 full videos for testing and schedule comparison

## CNN model

The CNN model was designed to classify frames and detect the end of Phase 4. The model included:

- Data augmentation layer
- Convolutional layer
- Max pooling layer
- Flatten layer
- Dense layers
- Dropout layer
- Output layer

The paper reports that Optuna was used for hyperparameter optimization, including learning rate, batch size, filter configuration, and dropout value.

## Dynamic scheduling logic

The scheduling logic can be summarized as follows:

1. Start the surgical video stream.
2. Capture a frame at regular intervals.
3. Classify the frame using the CNN.
4. If the frame does not indicate the end of Phase 4, continue monitoring.
5. If the frame indicates the end of Phase 4, record the elapsed time.
6. Update the OR schedule.
7. Prepare the next patient and supporting resources.

## Model evaluation

The model was evaluated using:

- Accuracy
- Specificity
- Sensitivity
- Precision
- Negative predictive value
- Confusion matrix
- ROC curve

The ROC curve reported an AUC of **0.95**, showing strong classification performance.
