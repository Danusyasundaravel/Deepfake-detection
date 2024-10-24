# DETECTION OF FACE-SWAP BASED DEEP FAKE VIDEOS DATA USING DEEP LEARNING

Deepfakes are manipulated videos where the faces of people are replaced with computer-generated likenesses. This project aims to detect such manipulations by leveraging machine learning models trained on video datasets containing real and fake videos.

## MODELS UTILIZED IN THIS PROJECT

2D CNN: Analyzes individual video frames.

3D CNN : Captures both spatial and temporal patterns from sequences of frames.

EfficientNet: A state-of-the-art image classification model that efficiently balances accuracy and performance.
## DATASET
The dataset used for this project is organized into two categories:

Real videos: Videos that contain unmanipulated footage.
Fake videos: Videos where faces have been digitally altered.
Each video is pre-processed by extracting frames and resizing them for input into the models.

## MODEL ARCHITECHTURE
### 2D CNN
This model processes individual frames of a video to detect deepfakes by analyzing spatial features. It's suitable for image-level classification but does not take into account the temporal relationship between frames.

### 3D CNN
Combines 3D CNNs for spatial feature extraction across multiple frames and LSTMs to learn temporal patterns, which is crucial for videos. This model can capture subtle temporal manipulations in videos.

### EfficientNet
EfficientNet is a pre-trained model used for image classification. It is efficient and achieves high accuracy with a relatively small number of parameters, making it ideal for detecting deepfakes in individual frames.

## MODEL COMPARISON

The 2D CNN model is basic and may miss subtle temporal artifacts, but is fast.

The 3D CNN model is better for deepfake detection due to its ability to capture both spatial and temporal changes in the video.

The EfficientNetB0 model provides a high-performing baseline by leveraging transfer learning, but it primarily focuses on spatial features unless combined with temporal methods which are mentioned in research papers.
