# Assignment: What Does My Neural Network Think?
Make a short video with your phone and generate a heatmap demonstrating why the neural network makes a particular prediction. 

### Objective
To understand the reason behind a prediction a neural network makes in object classification.
### Protocol
In order to generate a heatmap for a video taken by a phone camera, there are two steps needed:
1. Data collecting: a video of random kitchen objects is taken.
2. Create a folder in the directory path with ```!mkdir kitchen```
3. ```ffmpeg``` is called to split the input video into image frames in the folder 'kitchen'.
4. ```visualization.py``` is run to convert the plit image frames into heatmap images. [visualization.py](https://github.com/practicaldl/Practical-Deep-Learning-Book/blob/master/code/chapter-2/visualization.py) is a script essentially for video processing provided by [Practical Deep Learning](https://github.com/PracticalDL/Practical-Deep-Learning-Book/tree/master/code/chapter-2#readme) that produces the heatmap for images as well as videos. The ```vggg16 model``` is trained on ImageNet to make predictions.
5. Lastly, compile a video out of the processed frames.

### Results
- Input Video: [IMG_7576.MOV](https://github.com/van-anh-nguyen/Abgabe-2/blob/main/data/IMG_7576.MOV)
- Output Video: [kitchen-output.mp4](https://github.com/van-anh-nguyen/Abgabe-2/blob/main/data/kitchen-output.mp4)
- Input frames of video: [kitchen](https://github.com/van-anh-nguyen/Abgabe-2/tree/main/data/kitchen)
- Output frames of video: [kitchen-output](https://github.com/van-anh-nguyen/Abgabe-2/tree/main/data/kitchen-output)

### Source
- Anirudh, Koul, Ganju, Siddha and Kasam, Meher, Practical Deep Learning for Cloud, Mobile & Edge, Real-World AL & Computer Vision Projects Using Python & TensorFlow, O'Reilly Media, Inc., ISBN: 9781492034865, October 2019
- Github: [Practical Deep Learning, Chapter 2](https://github.com/PracticalDL/Practical-Deep-Learning-Book/tree/master/code/chapter-2#readme)
