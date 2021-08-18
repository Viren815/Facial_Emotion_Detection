Name : Viren Shah <br>
Id: 1152974 <br>
University: Lakehead University <br>

# Facial_Emotion_Detection
# Introduction 
<p>Face Emotion has become the most essential part of any conversation, whether the conversation is formal or informal. Although we can speak verbally, there are much more things that can be understood through facial expression. With the proliferation in technologies and advancement in Artificial Intelligence, predicting emotions became easier than ever. But there were still some doubts regarding how the computer will understand those emotions. Such issues were resolved with the help of Deep learning algorithms. With the help of Convolution Neural Network(CNN) and Deep Neural Network(DNN), the computer will be able to understand and predict different emotions.</p>  
<p>In this research, I have used four pretrained models with transfer learning ImageNet to predict the emotion. Those four classifiers are:-
<ol>
  <li>VGG-19</li>
  <li>ResNet-152</li>
  <li>MobileNet</li>
  <li>DenseNet-169</li>
</ol>
All four architecture are used to train the whole network individually and at the end, their accuracies are compared. There are some previous works in this field but they never try to enhance the dataset images or never used any pretrained model except VGG. Therefore, in this project, I tried to fill those gaps and train the whole model with these 4 classifiers to achieve the desired accuracy.  
</p>

# Dataset
<p>For this project, <a href="https://www.kaggle.com/deadskull7/fer2013">FERC-2013</a> dataset is used. The dataset is available as a csv file. It consist of approximately 36000 gray-scale images. It has low resolution as the size of each image is 48 x 48 pixels. It consists of seven categories of emotion such as Happy, Anger, Sad, Disgust, Fear, Surprise, Neural. </p>

# Requirement
Following are the required libraries to run the program:-
<ol>
  <li>Keras</li>
  <li>Tensorflow</li>
  <li>Sklearn</li>
  <li>Pandas</li>
  <li>os</li>
  <li>numpy</li>
  <li>Matplotlib</li>
</ol>

# How to Run this Project
<ul>
  <li> The project can be ran in Colab / Jupyter notebook </li>
  <li> Before running the project change the path of the given dataset </li>
  <li> Also change the runtime to GPU to run this project faster </li>
</ul>

# Implementation
 ![RM](https://user-images.githubusercontent.com/44722997/129968105-ed7e6495-6cab-432e-925e-c5d85f34e658.png)<br>
<p>
Starting with the implementation, firstly I am importing the dataset and performing pre-processing steps. In pre-processing, Normalization, Grayscale to RGB, and Resizing of each image is done. As I mentioned above that in the previous work of this field neither anyone tried to enhance the dataset by converting grayscale image into RGB nor tried to resize the image for high resolution. Therefore I am resizing the image from 48x48 pixels to 128x128 pixels. After then I am using 4 pretrained models along with the ImageNet database for feature extraction and finally training the whole network. At last, testing takes place where all the testing images are predicted.</p>

# Results
The below image displays the results attained after performing thorough research in the field and the outcomes from the proposed implementation <br>

 ![CV Presentation (1)](https://user-images.githubusercontent.com/44722997/129967704-d318fca8-eefc-4bae-8776-7bdcf0b55755.png)
 
# Conclusion 
The project compares different pretrained models of deep learning for facial emotion detection and determines which model can predict emotions better. Thus, this method may also assist other researchers or developers in creating a model which has the high computational power to predict features more precisely. 
  
