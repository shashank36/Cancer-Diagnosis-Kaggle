# Personalized-Cancer-Diagnosis

A lot has been said during the past several years about how precision medicine and, more concretely, how genetic testing is going to disrupt the way diseases like cancer are treated.  But this is only partially happening due to the huge amount of manual work still required. Memorial Sloan Kettering Cancer Center (MSKCC) launched this competition, accepted by the NIPS 2017 Competition Track,  because we need your help to take personalized medicine to its full potential.
Once sequenced, a cancer tumor can have thousands of genetic mutations. But the challenge is distinguishing the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers). 

Currently this interpretation of genetic mutations is being done manually. This is a very time-consuming task where a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.

For this competition MSKCC is making available an expert-annotated knowledge base where world-class researchers and oncologists have manually annotated thousands of mutations.

## Procedure followed to solve this case study

###  Read Gene and Variation Data

###  Read Text Data

###  Splitt data into train, test and cross validation (64:20:16)

###  Prediction using a 'Random' Model

In a 'Random' Model, we generate the NINE class probabilites randomly such that they sum to 1
We obtained a Log loss of 2.47 on Test Data using Random Model 
###  Univariate Analysis

	Featurize this Gene, Variation and Text feature with One hot Encoding and Response coding.
###  Applying all the models with tf-idf features and Instead of using all the words in the dataset, using only the top 1000 words based of tf-idf values
 

After applying all the models with tf-idf features and using only the top 1000 words based of tf-idf values, Logistic Regression using One Hot Encoding with class balance has given 1.04 test logloss, which is the lowest, as compared to other models.

###  Apply Logistic regression with CountVectorizer Features, including unigrams, bigrams , tri_gram, 4_gram
 


###  Apply feature engineering techniques to reduce the log-loss to a value less than 1.0
Added Gene Feature Variation feature to improve the performance. And after some feature engineering, we managed to decrease the log loss below < 1



