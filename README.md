# Social-Media-Information-Extraction


Problem Statement:

Here we will be analyzing  tweets to extract what types of information is stored. This type of problem can be extended to those kind of problems where a company may ask to analyze their product tweets or regarding email/ marketing campaign. In this project we will perform step by step decomposition of tweets and will try to decode what story this data is conveying. 

Dataset:

The data set contains around 15000 tweets about demonitization in October '16. It contains information like the content of the tweet (text), when it is created, source, ID, screenName adn whether it is retweeted and if then how many times.For this project we will be focusing on mining the content part of the dataset as it contains all the information that we need. The dataset is unstructured. First we we will be preprocessing / clean the data set. 

Preprocessing:

Step 1: We will lowercase all the characters present. 
Step 2: Remove all the punctuations 
Step 3: Remove all the stop words. We will use NLTK corpus to get stopwords list present in "english" language. 


Analysis :

Following analyses can be done 

1. What are the major keywords used 
2. What are the phrases mentioned 
3. Who (people) are mentioned
4. What Email/ URLS are mentioned. 
5. Which hastags are used the most
6. Sentiment Analysis
7. Bigrams (which two popular words are used together the most)

KeyWords 

It will give which type of keywords are used the most
The top five in this dataset are as follows. 

demonetization, 13939
rt: 11059
india: 2766
modi: 2759
pm :  2729
narendra: 1566

Mentions 
We can see celebrity names, people from tech companies, politicians, ministry offices, news media etc. are mentioned. 

@evanspiegel:  1301
@URautelaForever: 1273
@narendramodi: 1059
@gauravcsawant: 541
@ModiBharosa: 539
@DrKumarVishwas:  350

In similar way we can see it for Hashtags
We can see "demonitization" is most mentioned hastags. Apart from demonitization, we can see other hastags used by removing demonitization
#Demonetization :  3030
#demonetization: 2241
#DeMonetization: 706
#demonetization: 704
#India: 286

Others
#India: 286
#nitishkumar: 257
#GLvMIRT: 120
#CorruptionFreeIndia: 103
#BlackMoney: 87

URL/ links mentioned: 
https://t.co/ObQrhlNSL6RT: 277
https://t: 252
https://t.co/UodwXdPMmGRT:  204

Bigrams (two words together)

Importing ngrams from nltk, we can top bigrams present in the dataset. 

narendra, modi: 1565
india, rich: 1431
pm,narendra: 1424
demonetization, find: 1399
implement, demonetization: 1397

People/ Organizations most mentioned :
It consists of variosu names, palces, organizations etc, depending upon the requirement we can segregate these. 
Some of them are given below

(ORGANIZATION PM/NNP)
(GPE Modi/NNP)
(ORGANIZATION RBI/NNP Dy/NNP)
(ORGANIZATION CBDT/NNP)
(PERSON Harvard/NNP Professor/NNP)
(PERSON Aam/NNP Aadmi/NNP)


