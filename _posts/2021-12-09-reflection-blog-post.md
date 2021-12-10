---
layout: post
title: "Mussic Classifier Project Reflection Blog Post"
date: 2021-12-09 01:00:00
---

### Overall, what did you achieve in you project?
*This section is written as a group*

 I love music, and I always regard music as a source of stress relief. It is a great experience for me to do a project related to music. Music is easy to access nowadays thanks to technology development and the internet. However, when downloading music to our own phone, there is no genre classification, and it is hard to get all of the downloaded songs sorted manually. So, after our discussion, we finally decided to develop a model which would solve this problem and get the song’s genre classified from its metadata. And we would like to implement the model into a webapp, which is more accessible to users and, at the same time, gives a more straightforward visualization of how our model works.


### What two aspects of your project that you are especially proud of?
* Incorporating the Spotify Web API 

We obtained the training/tesring/validation dataset on Kaggle, which naturally comes with the lyrics and feature values coloumns for the songs. However, when we construct the web app, we could only collect the user input as a song rather than a well modified dataset. In order to be able to pass our machine leanring model to the user input and predict the genre of a song, we came up with the idea of employing the Spotify Web API to convert user input into a dataset with different scalar value columns such as danceability, valence, energy, etc. 

* Implementating the machine learning model to the web app 

Our team encountered several problems in implementing the machine learning model to the web app. Since we worked on the google colab, we had an issue in downloading the model to the local laptop. Then we encountered difficulties in calling the Keras model on our dataset transformed from the user input since the columns do not match with our training data. After hours of debugging and also with the help of our TA and professor, we have finally successfully implemented our model to the web app!

### What are two things you would suggest doing to further improve your project?
* Improving web app user input:

In our web app, we ask the user to input a song's Spotify ID and lyrics of the song. However, manually copying and pasting lyrics on third-party websites could be time-consuming and inconvenient. Therefore, one improvement for our project would be automatically generating the lyrcis of a song once the user inputs the song id in order to improve the user experience. 

* Supporting songs in languages other than English:

Currently our project only supports for music classification of English songs, and there might be bias in classifying genres when the training dataset only consists of English songs. We would also like to incorporate other languages to serve a broader audience.

### How does what you achieved compare to what you set out to do in your proposal?
*This section is written as a group*

 Our planned deliverables:
 We aim to create a webapp finally to classify the genre and identify the sentiments of a song. The webapp will be able to classify the genre and sentiments of a song by reviewing the lyrics. A classification model would be trained by us and implemented to the webapp.

 Compared to our plan, we have actually achieved almost all parts that we set out to do! We successfully build the genre classification model and create the web app interface. One slight difference is that we decided not to the include the sentiment analysis section but go with a more accurate and applicable way to construct the genre classification part by implementing the model to a mixed feature dataset (lyrics + scalar feature columns).


### What are three things you learned from the experience of completing your project? Data analysis techniques? Python packages? Git + GitHub? Etc? 
* Git + GitHub!

I personally have not used GitHub before. It is really a useful tool to collaborate and develop a project with other people.

* Python package: Tensorflow

Since the main goal for our project is to construct a machine learning model to classify genres of songs, I really learned a lot about how to use Tensorflow to build a model and try various layers on mixed feature dataset to improve the validation accuracy of the model. 


* Python package: Flask

In class we were introduced to the basics of developing web app using flask and did a blog post on this topic. In completing my project, I got a further taste in how web app building works and how to import models and pass other functions such as Spotify web API to transform the user input into data forms that we want. 


### How will your experience completing this project will help you in your future studies or career?
Tools we used in completing this project, such as text classification and tensorflow maching learning algorithm, are very useful and practical for careers related to data science and data analysis. Topics such as natural language processing are also very popular fields. Most importantly, skills such as working in a team and expanding the knowledge learned in class to develop interesting applications are definitely helpful for my future studies and career!












