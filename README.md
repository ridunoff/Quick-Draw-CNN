# Quick-Draw-CNN
A convolutional neural net that classifies images from Google's Quick, Draw! dataset.

## Project Description

Our project could be used as a part of a drawable-search feature for the emoji keyboard. When designing this model, we had to consider the different representations of emojis across platforms and also the different interpretations of representing a word visually. 

 <img src="images/openBook.png" height="200">       <img src="images/closedBook.png" height="200"> 

One consideration was that people can interpret a book to be draw as either an open book or a closed book. The CNN should be able to understand both interpretations.

<img src="images/differentEmojis.png" width="300"> Apple Emoji (Left) Google Emoji (Right)


Another consideration was that operating systems can vary in the way they represent emojis (Apple vs Google emoji Keyboards). These differences are converging however some discrepencies still remain.

Since our product would be more of a novelty feature of a phone's keyboard, it would be fine with a non-perfect level of accuracy. The stakeholders would be people who are new and unfamiliar with the emoji keyboard, so adults that are new to technology, but also good at drawing. One risk of our algorithm not working properly would be frustration of sadi adults with needing to scroll through the enrire emoji keyboard to find the emoji they are looking for.


## The Data

We used drawings from [Google's Quick, Draw!](https://quickdraw.withgoogle.com/data) dataset. 

 <img src="images/airplaneHeatmap.png" width="400"> 

The drawings were represented as a 28x28 heatmap

We deliberatly chose datasets that looked different from each other in order to create a more accurate model to validate that our algorithm could work to classify images.

The datasets we chose were: airplane, basketball, bee, bicycle, butterfly, cookie, helicopter, lightbulb, pants, and strawberry.


## The Results

The model was able to correctly guess images within a resonable margin of error!

 <img src="images/test_image.png" width="400"> 

![Results](images/confidence_plt.png)

We also discoved that 5000 images in the training set gave us around 79% accuracy of correctly classifying the drawing in the testing data set. The training accuracy was around 82% accurate.

![Modeled Loss](images/test_train_loss.jpg)

This Confusion Matrix shows the actual and predicted results of our algorithm.

![Confusion Matrix](images/confusion_matrix.png)



