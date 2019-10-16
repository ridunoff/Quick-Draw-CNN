# Quick-Draw-CNN
A convolutional neural net that classifies images from Google's Quick, Draw! dataset.

## Project Description

Our project could be used as a part of a drawable-search feature for the emoji keyboard. When designing this model, we had to consider the different representations of emojis across platforms and also the different interpretations of representing a word visually. 

 <img src="images/openBook.png" width="200"> ![Closed Book Drawing](images/closedBook.png) 

Some people can interpret a book to be draw as either an open book or a closed book. The CNN should be able to understand both interpretations.

![Different Emojis](differentEmojis.png)  { width: 200px; } 

Some operating systems can vary in the way they represent emojis (Apple vs Google emoji Keyboards). These differences are converging however some discrepencies still remain.


## The Data

We used drawings from [Google's Quick, Draw!](https://quickdraw.withgoogle.com/data) dataset. 

![Drawing of a Airplane](/images/airplaneHeatmap.png) { width: 200px; }

The drawings were represented as a 28x28 heatmap

We deliberatly chose datasets that looked different from each other in order to create a more accurate model to validate that our algorithm could work to classify images.

The datasets we chose were: airplane, basketball, bee, bicycle, butterfly, cookie, helicopter, lightbulb, pants, and strawberry.


## The Results

The model was able to correctly guess images within a resonable margin of error!

![Drawing of an Airplane](images/airplaneHeatmap.png)

![Results](images/airplaneResults.png)

We also discoved that 5000 images in the training set gave us around 81% accuracy.

![Modeled Loss](images/test_train_loss.jpg)

This Confusion Matrix shows the actual and predicted results of our algorithm.

![Confusion Matrix](images/confusion_matrix.png)



