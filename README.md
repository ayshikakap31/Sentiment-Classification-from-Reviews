# Sentiment-Classification-from-Reviews
This project aims to classify the sentiment of human generated IMDB movie reviews as either positive or negative labels. As, neural networks don't accept text inputs directly so, we'll have to transform the textual inputs data to numerical form so that the neural networks can discover correlation. 
The file 'reviews.txt' consists of 25000 movie reviews and 'labels.txt' consists the corresponding label as POSITIVE or NEGATIVE.
At first, we did a theory validation by finding words that are most common in POSITIVE and NEGATIVE reviews. It can be observed that there are few words that are common in both. So, we found ratio between words that are commo between both labels.
Next, we transformed the text into numbers. We converted each review string into a vector that uses the counts of each word in the review as input to the neural network. Also, for output the NEGATIVE is transformed to '0' and POSITIVE to '1'.
Then, a basic 3 layer neural network is built. There is no non-linearity in the hidden layer. Also, a function to pre-process our training data is created.
