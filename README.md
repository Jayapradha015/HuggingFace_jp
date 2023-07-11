Sentimental Analysis on Reviews using TextBlob and HuggingFace Transformers


Dataset:
     The data is about reviews of the earphone and this data has been scraped from the amazon website using the request library. 
The raw data is parsed using the beautifulsoup library. From the entire page content, the reviews are extracted using Python. 
Then the final data is converted into a pandas data frame.

Data Preprocessing for NLP:
      Data preprocessing for NLP tasks is important, and I have used the nltk library for that. Basics steps like removing emoji, 
lemmatization, stopwords, and tokenization are done using nltk. The final output of this process is clean text that can be used for 
sentimental analysis.

TextBlob:
      The first library I have used is Textblob. This library processes the data and finds the polarity of the review. 
It gives the polarity score. Using the polarity score we can assign the category to each as positive, negative, or neutral.
If the score is greater than zero then it is positive, if it is less than zero then it is negative and 
if it is equal to zero then it is neutral.


Roberta pretrained model:
      This model is from the hugging face transformers library. This model is a pretrained one, we can use this model to finetune our
dataset. The important feature of this Roberta model is, it tokenizes the sentence into words based on the context it is used. 
Based on this factor the words are selected for the analysis of the polarity of the sentence. After that, the sentence is assigned with
Positive, Negative, and Neutral categories.



Comparision of TextBlob and Roberta model:
      The comparison is based on the categories assigned by these models to each sentence. As both these models have different 
ways of analyzing the data, the sentiments assigned by these models are different in some of the sentences.
eg.
   Sentence: "The touch and other functions are fine but the sound quality is just bad, reason why I'm returning the product."
   The sentiment of TextBlob: positve
   The sentiment of Roberta: Negative

 
