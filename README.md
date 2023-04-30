# Sentiment-Classification-from-Reviews
This project aims to classify the sentiment of human-generated IMDB movie reviews as either positive or negative. Since neural networks don't accept text inputs directly, we needed to transform the textual input data into a numerical form so that the neural networks could discover correlations.

The project uses two files, 'reviews.txt' and 'labels.txt', consisting of 25,000 movie reviews and corresponding labels as POSITIVE or NEGATIVE. Before building the neural network, we validated the theory by finding the most common words in POSITIVE and NEGATIVE reviews. We observed that only a few words were common in both, so we found the ratio between words that were common between both labels.

Next, we transformed the text into numbers. We converted each review string into a vector that used the counts of each word in the review as input to the neural network. Additionally, we transformed NEGATIVE to '0' and POSITIVE to '1' for output.

We then built a basic three-layer neural network. The hidden layer does not have any non-linearity. We also created a function to preprocess our training data to reduce noise in the input data, which made the training faster and improved the accuracy of predictions.

To further optimize the network, we analyzed inefficiencies in our network by eliminating unnecessary multiplications and additions that occur during forward and backward propagation. Finally, we improved the network's performance by strategically reducing more noise in the vocabulary.

Overall, this project provides a solution to classify the sentiment of movie reviews using a basic three-layer neural network and pre-processing techniques to reduce noise and optimize the network's performance.

## Installation
To use this project, you will need to install the required dependencies, including Python, numpy, time, sys, matplotlib, sklearn.

##Usage
To use the sentiment classifier, run the 'Solution.ipynb' script.
