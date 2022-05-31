# Assignment: What Does My Neural Network Think?
Make a short video with your phone and generate a heatmap demonstrating why the neural network makes a particular prediction. 

### Objective
To understand the reason behind a prediction a neural network makes in object classification.
### Description
In order to generate a heatmap for a video taken by a phone camera, there are two steps needed:
1. Data collecting: a video of random kitchen objects
2. Create a folder called "kitchen" in the directory path with ```!mkdir kitchen```
3. ```ffmpeg``` is called to split the input video into image frames and save them in the folder 'kitchen'.
4. ```visualization.py``` is run to convert the plit image frames into heatmap images. [visualization.py](https://github.com/practicaldl/Practical-Deep-Learning-Book/blob/master/code/chapter-2/visualization.py) is a script essentially for video processing provided by [Practical Deep Learning](https://github.com/PracticalDL/Practical-Deep-Learning-Book/tree/master/code/chapter-2#readme) that produces the heatmap for images as well as videos. The ```vggg16``` model is trained on ImageNet dataset to make predictions.
5. Lastly, compile a video out of the processed frames. Output should be the original video but in heatmap form.

### Results
- Input Video: [kitchen-input.MOV](data/kitchen-input.MOV)
- Output Video: [kitchen-output.mp4](https://github.com/van-anh-nguyen/Abgabe-2/blob/main/data/kitchen-output.mp4)
- Input frames of video: [kitchen](https://github.com/van-anh-nguyen/Abgabe-2/tree/main/data/kitchen)
- Output frames of video: [kitchen-output](https://github.com/van-anh-nguyen/Abgabe-2/tree/main/data/kitchen-output)

### Sources
- Anirudh, Koul, Ganju, Siddha and Kasam, Meher, Practical Deep Learning for Cloud, Mobile & Edge, Real-World AL & Computer Vision Projects Using Python & TensorFlow, O'Reilly Media, Inc., ISBN: 9781492034865, October 2019
- Github: [Practical Deep Learning, Chapter 2, What Does My Neural Network Think?](https://github.com/practicaldl/Practical-Deep-Learning-Book/blob/master/code/chapter-2/2-what-does-my-neural-network-think.ipynb)
