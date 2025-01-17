# ✋ Finger Counting with OpenCV
## 📖 Introduction
Counting fingers is a common task in computer vision, useful for gesture recognition. Here, we compare edge detection + contour methods with deep learning approaches.
After implementing finger counting using edge detection and contours with OpenCV, I'll try using deep learning for this project. Afterward, I will compare the two methods.<br>
📊 Dataset: [🔗 View the Dataset on Kaggle](https://www.kaggle.com/datasets/koryakinp/fingers)<br>
The dataset contains 21,600 images of left and right hands, with finger counts from 0 to 5. All images are 128x128 pixels.
![Dataset Cover](Image/dataset-cover.jpg "5 image classes of Fingers") 

## 🧠 Results with Basic CNN
<img src="Image/CNN_test.gif"/>
As we can see, it's still not perfect, even though the model achieved an accuracy of over 96% and a loss of less than 1% on test images. But it's still better than traditional method that can't predict in dim lights, but with Deep Learning it's more achieveable. 

## ❌ Problems
🟥 The model may make incorrect predictions if the angle of the captured fingers differs from the dataset.<br>
🟥 The model will make incorrect predictions if the background is not blank.
## 🛠️ How to Solve These Issues
🔲 Process the dataset to make it more like binary threshold images and train the model using that dataset.<br>
🔲 Try different model architectures or use a pretrained model with the ImageNet dataset, hoping that it can be better at classifying images<br>
🔲 Add more images to the dataset by recording my own fingers and labeling them.<br>
🔲 Try different data augmentation techniques and find the best way to augment the dataset.
