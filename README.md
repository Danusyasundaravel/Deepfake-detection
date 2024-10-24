# Deepfake-detection
Deepfakes are manipulated videos where the faces of people are replaced with computer-generated likenesses. This project aims to detect such manipulations by leveraging machine learning models trained on video datasets containing real and fake videos.

## Three models are utilized in this project:

2D CNN: Analyzes individual video frames.
3D CNN + LSTM: Captures both spatial and temporal patterns from sequences of frames.
EfficientNet: A state-of-the-art image classification model that efficiently balances accuracy and performance.
## Dataset
The dataset used for this project is organized into two categories:

Real videos: Videos that contain unmanipulated footage.
Fake videos: Videos where faces have been digitally altered.
Each video is pre-processed by extracting frames and resizing them for input into the models.

## Model Architectures
### 2D CNN
This model processes individual frames of a video to detect deepfakes by analyzing spatial features. It's suitable for image-level classification but does not take into account the temporal relationship between frames.

### 3D CNN + LSTM
Combines 3D CNNs for spatial feature extraction across multiple frames and LSTMs to learn temporal patterns, which is crucial for videos. This model can capture subtle temporal manipulations in videos.

### EfficientNet
EfficientNet is a pre-trained model used for image classification. It is efficient and achieves high accuracy with a relatively small number of parameters, making it ideal for detecting deepfakes in individual frames.
