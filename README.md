# Movie-Genre-Prediction-using-CNN
Multi-Label Image Classification on Movies Poster using CNN
Topic: Multi-Label Image Classification on Movies Poster using CNN 

Title: “Can a Machine Predict the Genres of a Movie from it’s Poster?”


Making an image classification model is a good start, but we wanted to take it up a notch and expand our horizons. Hence instead of a multi-class model we decided to build a multi-label image classification model where there are multiple objects in a single image thus multi-label.

 

Next, we had to decide what kind of images we would like to classify which like mentioned before could have multiple objects to label in them, and while the answer was right in front of us, we did have a discussion and being movie enthusiasts and having argued a lot on genre of the movies it only made sense to build a model which could prove which one was right at the end of the day. A movie usually belongs to multiple genre that means more than one genre and not necessarily belong to one category like drama or thriller. So, the question was, could we build our own multi-label image classification model to predict the different genres just by looking at the poster?  Keep reading to find out.
 

Project Objective:
The objective of our project is to predict the genre of a movie using its poster image. 
A movie usually belongs to multiple genre that means more than one genre and not necessarily belong to one category like drama or thriller. Most of the times a movie is a combination of more than one genre. Hence, we are doing multi-label image classification here. The CNN model we will make, will be classifying a poster among 25 different genres based on its processing of the image and classify it to the appropriate genre of that movie. In the end, our CNN model should predict the genre of a movie judging from its poster. 

Information About the Dataset:
Dataset Link: https://www.kaggle.com/raman77768/movie-classifier#  
This dataset was collected from the IMDB website. One poster image was collected from one (mostly) Hollywood movies released from 1980 to 2015. Each poster image is associated with a movie as well as some metadata like ID, genres. The ID of each image is set as its file name.
The dataset contains 7254 rows and 27 columns along with the movie’s posters. 

First, we picked up a dataset related to movie posters having 25 different genres for labels and started working on it. Secondly, we preprocess the data in order to make it readable to the system. Then we built a CNN architecture model and trained the model on the training dataset later validated on the testing dataset. Though we achieved an accuracy of 90% for our model, the hardest aspect of the model building was to avoid overfitting rather than achieving a greater accuracy. To overcome this problem, we retrained our model several times by removing neural layers and reducing the number of elements in hidden layers which are present typically in any CNN architecture. After working on it for 2 days we finally got our desired model.


The validation accuracy (around 90%) is almost same with the training accuracy and the same with the validation loss. Hence, the model is working fine but may have overfitting problem as dataset was biased.
If a certain genre is repeating in most of the training images, the model may overfit on that genre. And for every new image, the model may predict the same genre. To overcome the overfitting this problem, the dataset should have an equal distribution of genre categories.
Testing of the Model

So, how does our model work? Generally, our model will give the probability of all 25 genre for each poster that you feed to the model but we are only interested in the top 3 genres of that Movie/TV series poster. As shown below.
  

Further we created a web app that has a user-friendly interface, where you will just upload a poster and it will give you the top 3 predicted genres of that poster.
Video recording link: Analytics Project
 
 
 
Next Step Ahead 
The project can be modified to have different other functionalities starting off with a recommendation system which works based on genre filters and favorite characters in the films poster. It can also be modified to aid the designers by recommending the right color scheme to be used and the various elements that can be put up in the poster in order to portray the correct genre. It can also be used by the marketing team to analyze whether the poster made by the designers conveys the correct idea. Hence helping both sides of the businesses make decisions accurately.

So, having done all things what did we achieve?  Let’s ANALYSE. We learnt how to write a ton of code, how to implement CNN models for image classification, how we can get genre information by just a click of a button and a lot of other backend work.
