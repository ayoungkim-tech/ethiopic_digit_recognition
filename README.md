# ethiopic_digit_recognition
https://github.com/ayoungkim-tech/ethiopic_digit_recognition  
It is [Kaggle competition](https://www.kaggle.com/c/tau-ethiopic-digit-recognition) project work from the course.  
The method used at here is CNN with a dense layer with softmax activation as the last layer.
# Tech/framework used
Built with [Jupyter Notebook ](https://jupyter.org/) using Python programming language.
# Features
   Softmax regression is a model that can classify into n different classes. Logistic regression only classifies into two different classes. Compared to Logistic regression, using a dense layer with softmax activation as the last layer of our CNN model is more suitable for the classification of Ethiopic digits. It is because we can interpret output as the probability of the image belonging to one of the ten classes.  

   Initially, we used 2 convolutional layers without data normalisation. In order to improve preliminary results we normalised the data, this helps the model to converge faster. Additionally, we increase the number of convolutional layers to 3 which help the model to learn more abstract information from the images that could help the classification objective. We did also tested two optimisers: "adam" and "rmsprop", being the later the one with better performance in our experiments. Finally, we trained our model for 30 epoch from which we obtained an accuracy of 0.9824 on Kaggle leaderboard, to increase this accuracy we trained our model for 60 epochs. Using this strategy, the neural network was able to improve the accuracy to 0.9936 on Kaggle leaderboard. If we try a higher epoch value, the accuracy can be imporved more, but it might be overfitting.
