# Cross-Lingual-Embedding
E​ valuated the Facebook MUSE cross-lingual word embeddings

Final Project of the Advance Data Mining class at Illinois Institute of technology, Spring semester 2019.

Team of 4 People : **Chandana Ravindra Prasad, Sandeep Fnu, Inigo Alonso Gago, Thomas Ehling**

## Abstract

We consider the problem of performing binary sentiment analysis on Spanish movie reviews using the MUSE
cross-lingual embeddings and an LSTM network trained on an English dataset. Because data is scarce in foreign
languages, the most common method remained using direct translation. ​ We use datasets from 2 different
sources and the more generalized 50_00 embeddings. ​ Our model scored an accuracy of ​ 72.97% on the
Spanish reviews, against 87.56% on English reviews. This result shows that is possible to obtain a
correct accuracy on reviews from a different source and language without translation. It brings a lot of
new opportunities in a field needing huge amounts of data.

## Link to the MUSE Embeddings official page
MUSE embeddings GitHub :
https://github.com/facebookresearch/MUSE

## Implementation :

The zipped /data folder, with the MUSE embeddings, model weidths, clean datasets and pickle file for the vocabularies is accessible throught this link : https://drive.google.com/file/d/1VSn4Pp4QOn4ipLF7GNSrJY5A2DcyOTNt/view?usp=sharing

**CAREFUL : Due to the Embeddings the /data folder is huge once unzipped : 1.7GB"**

If you wish to implement our code, and recreate our result, do the following steps :

**A. On Google Drive :**
  1. download and unzip the "data" folder
  2. copy the "data" folder to your drive.
  3. Add these the two files to the /data folder
  4. Upload "Cross_Lingual_Embeddings.ipynb" and open it with colab
  5. In the 4 line, change the PATH_DRIVE to your path to the /data folder
  6. Run "Cross_Lingual_Embeddings.ipynb"

**B. Localy :**
  1. download and unzip the "data" folder
  2. Open "Cross_Lingual_Embeddings.ipynb"
  3. delete the first two line of code
  4. change the PATH_DRIVE value to your local path to the /data foler
  5. Run "Cross_Lingual_Embeddings.ipynb"

## Result :

Here are a table with our final results.

| MUSE embeddings  |  Test set | Accuracy  |
|---|---|---|
| NO  | IMDB  | 86.94%  |
| YES  | IMDB  | 87.56%  |
| YES  | Corpus Cine Translated  |  87.26% |
| YES  |  Corpus Cine | 72.97%  |

The first 3 rows represent a baseline to compare our result to.
The last one is the final performance of our model on the row Spanish data.

## Conclusion

Multilingual techniques, including Cross-lingual word embeddings, are an active area of research, full of opportunities. Only a few weeks ago, the Amazon Alexa team released a paper on multilingual text classification with word embeddings, character embedding, and several deep neural networks architectures.

The specificity of this project was to show the efficiency of the MUSE embeddings, using only the 50_000 most general ones and training and testing on two datasets from different language but also different sources.  Even with all these challenges, we still ended up with a high accuracy of 73%, 15% different from the testing on English data. Our result proves that we can use the MUSE embeddings to classify an unseen dataset in a new language.
  
This is really exciting. These MUSE Embeddings have been made available by Facebook, so we can predict a future where the machine Learning model can be developed and trained by large companies like Amazon, on their billions of reviews, and we could use these model to classify any document in any language! This is an even more amazing breakthrough as we need new translation technique with the world globalization and immigration status, and it can bring new discoveries in languages that were not accurately useable due to the scarcity of the data.


## Final report like a research paper

We conducted a thorough error analysis, explained in details our decisions and the big picture behind this project in a report written with the same constraints as a research paper.

THis final report can be found here : https://github.com/ThomasEhling/Cross-Lingual-Embedding/blob/master/Cross_Lingual_Embedding_Report.pdf

or in this repository as the "Cross_Lingual_Embedding_Report.pdf" file.


