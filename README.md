# Sentiment-Classification-from-Reviews
This project aims to classify the sentiment of human generated IMDB movie reviews as either positive or negative labels. As, neural networks don't accept text inputs directly so, we'll have to transform the textual inputs data to numerical form so that the neural networks can discover correlation. 
The file 'reviews.txt' consists of 25000 movie reviews and 'labels.txt' consists the corresponding label as POSITIVE or NEGATIVE.
At first, we did a theory validation by finding words that are most common in POSITIVE and NEGATIVE reviews. It can be observed that there are few words that are common in both. So, we found ratio between words that are commo between both labels.
Next, we transformed the text into numbers. We converted each review string into a vector that uses the counts of each word in the review as input to the neural network. Also, for output the NEGATIVE is transformed to '0' and POSITIVE to '1'.
Then, a basic 3 layer neural network is built. There is no non-linearity in the hidden layer. Also, a function to pre-process our training data is created.
To make the training faster and to improve accuracy of predictions, we reduce the noise in the input data.
To further optimize our network, we analyze inefficiencies in our network by eliminating unnecessary multiplications and additions that occur during forward and backward propogation.
Lastly, we imporove the network's performance by reducing more noise strategically in the vocabulary.
