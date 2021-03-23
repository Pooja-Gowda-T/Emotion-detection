# Emotion-detection
Emotion-detection
This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML).
This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

# DEPENDENCIES

1. Python 3
2. OpenCV
3. Tensorflow
4. To install the required packages, run pip install -r requirements.txt.

# USAGE

 If you want to train this model, use:

* cd src
python emotions.py --mode train

If u want to view the prediction without training then use:

* cd src
python emotions.py --mode display

# ALGORITHM

1.First, the haar cascade method is used to detect faces in each frame of the webcam feed.

2.The region of image containing the face is resized to 48x48 and is passed as input to the CNN.

3.The network outputs a list of softmax scores for the seven classes of emotions.

4.The emotion with maximum score is displayed on the screen.



