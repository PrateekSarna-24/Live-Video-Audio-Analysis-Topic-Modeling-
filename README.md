# Live-Video-Audio-Analysis-Topic-Modeling-
### Note 
1. Every peice of code in this File has written During the Hackathon.
2. The Dataset used is UCF-101 is of 6GB.UCF101 - Action Recognition Data Set" which is a commonly used dataset for action recognition tasks. It contains videos of human actions collected from YouTube. The dataset is composed of 13,320 videos from 101 action categories. Each category contains at least 100 videos, and the total duration of the dataset is over 27 hours. It is frequently used for training and evaluating action recognition models and algorithms, especially in the field of computer vision and deep learning.
### This Project is Devided into 2 Parts
1. Video Temporal Analysis
2. Audio Analysis by Topic Modeling
### Project Explanation
#### Vision
To achieve a way to instantly remove or stop a live video by analyzing if there is any bad content.
#### How to Achieve?
1. Analysis of any live video could be done in both visual and audio formats.
2. So the Project is Devided into 2 parts first is video analysis and 2nd is Audio Analysis.
#### Limitation
1. The limitation for this project is that there is no VULGAR dataset publicaly available.
2. Also, since the data is very big to process and require a lot of computaional power, I will just be using a portion of data and upto 2 categories / classes.
#### Solution
1. So to solve this drawback I am using a genric dataset with day to day actions performed by humans. These are generally the things such as "Applying Makeup", "Writing on a board".
2. For now the approach is to train the model with good data and see how the model performs, if the required dataset becomes available the model would be retrained according to it.
#### Approach
1. For Video
   
a. Using a pre-trained 3D CNN model for video data processing.Using R(2 + 1)D

b. Video = Sequence of Frames(Images)

c. Using the Sequence of frames to predict the category of action.

2. For Audio
   
a. I will extract audio from the video itself.

b. Then I will be converting the audio file to text file.

c. Then I will use Topic Modeling to get different patterns.

d. And then analyze those patterns to find any anomaly.

#### Main Libraries used
1. OpenCV
2. PyTorch
3. SpeechRecogniton
4. Librosa
