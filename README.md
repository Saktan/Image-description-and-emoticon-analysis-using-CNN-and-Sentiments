# Image description and emoticon analysis using CNN and Sentiments

In this , we have used CNN with LSTM as our model for predicting caption on a given image set. In variation to previous implementations, we have introduced an emoji in our caption to make it look more attractive and social. Firstly, we processed the image through pre-trained model VGG16 and mapped the output with decoder containing different layers of LSTM. The decoder then results in the output in the form of text. After getting the text, we applied sentimental analysis to our text which results in output as a sentiment. These sentiments are then mapped with emojis to get the caption with emoji. The dataset we used here is Flickr 8k. The result shows that the model performs very well.

Proposed Methodology

Import the dataset Flickr 8K and store it in the file from where you can save it in pandas data frame.
Cleansing of the caption is to be done i.e removing punctuation and higher frequency words(doesn’t contain important information).
Add two tokens named start and end in the captions.
Create features for the images by applying the pre-trained model VGC16 and Inception V3.
Mapped image with the respective text. Then change the character into integers for entering it into the model as the model accepts only integers.
Split training and testing data. Trained the model using training data.
Test the model and evaluate performance.
The generated text then passed for sentimental analysis which generates sentiments for a particular text.
The output sentiments are mapped with emojis. Then merge the emoticons with text for generating a better caption.




