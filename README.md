# Hand-and-finger-detection
# Emotion detection using deep learning

## Introduction

This project aims to help you track your hand.

## Dependencies

* Python 3, [OpenCV](https://opencv.org/)


## Basic Usage



* First, clone the repository and enter the folder

```bash
git clone https://github.com/atulapra/Emotion-detection.git
cd Hand and finger detection
```

* Download the FER-2013 dataset from [here](https://drive.google.com/file/d/1X60B-uR3NtqPd4oosdotpbDgy8KOfUdr/view?usp=sharing) and unzip it inside the `src` folder. This will create the folder `data`.

* If you want to train this model, use:  

```bash
cd src
python emotions.py --mode train
```

* If you want to view the predictions without training again, you can download the pre-trained model from [here](https://drive.google.com/file/d/1FUn0XNOzf-nQV7QjbBPA6-8GLoHNNgv-/view?usp=sharing) and then run:  

```bash
cd src
python emotions.py --mode display
```

* The folder structure is of the form:  
  src:
  * data (folder)
  * `emotions.py` (file)
  * `haarcascade_frontalface_default.xml` (file)
  * `model.h5` (file)

* This implementation by default detects emotions on all faces in the webcam feed. With a simple 4-layer CNN, the test accuracy reached 63.2% in 50 epochs.

![Accuracy plot](imgs/accuracy.png)

## Data Preparation (optional)

* The [original FER2013 dataset in Kaggle](https://www.kaggle.com/deadskull7/fer2013) is available as a single csv file. I had converted into a dataset of images in the PNG format for training/testing and provided this as the dataset in the previous section.

* In case you are looking to experiment with new datasets, you may have to deal with data in the csv format. I have provided the code I wrote for data preprocessing in the `dataset_prepare.py` file which can be used for reference.

## Algorithm

* First, the **haar cascade** method is used to detect faces in each frame of the webcam feed.

* The region of image containing the face is resized to **48x48** and is passed as input to the CNN.

* The network outputs a list of **softmax scores** for the seven classes of emotions.

* The emotion with maximum score is displayed on the screen.

## Example Output

![Mutiface](imgs/multiface.png)


<h1 align="center">Hi 👋, I'm Puneesh Gogia</h1>
<h3 align="center">A passionate Python developer from India</h3>

- 🌱 I’m currently learning **Tensorflow**

- 👨‍💻 All of my projects are available at [https://github.com/Puneesh6280](https://github.com/Puneesh6280)

- 📫 How to reach me **puneesh.gogia15@gmail.com**


<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.arduino.cc/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=puneesh6280&show_icons=true&locale=en&layout=compact" alt="puneesh6280" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=puneesh6280&show_icons=true&locale=en" alt="puneesh6280" /></p>






<h1 align="center">Hi 👋, I'm Puneesh Gogia</h1>
<h3 align="center">A passionate Python developer from India</h3>

- 🌱 I’m currently learning **Tensorflow**

- 👨‍💻 All of my projects are available at [https://github.com/Puneesh6280](https://github.com/Puneesh6280)

- 📫 How to reach me **puneesh.gogia15@gmail.com**


<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.arduino.cc/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=puneesh6280&show_icons=true&locale=en&layout=compact" alt="puneesh6280" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=puneesh6280&show_icons=true&locale=en" alt="puneesh6280" /></p>

