- first we should have the dataset which will contain different mails.
- once we have the dataset we are going to pre process the data.
- after pre-processing the data we are going to split the data into train data and test data . TRAIN DATA → is used to train the machine while TEST DATA → is used to measure the accuracy that how the machine is performing on the test data.
- in this project we have to check weather the mail is spam or not,  so we can say that it like binary classification like 0 or 1.
- so for this particular situation we will  use Logistic Regression Model because it perform well on binary classification.
- So, when you give a new mail to trained Logistic Regression Model it will predict weather the it is (spam mail) or (ham mail).
- from sklearn.feature_extraction.text import TfidfVectorizer purpose of this TfidfVectorizer we need to convert the text data in this text data is nothing but the mail data convert it into numerical value.  IF YOU JUST FEED THE TEXT DATA THE MACHINE LEARNING MODEL CANNOT UNDERSTAND.

This TfidfVectorizer try to go through all the words in your document  so in your in this the document is nothing but the data set we have. if the word is repeated several times it will get some values . so it is going to give some values or give some score to all the words that has been present in the data .

- So this important score or the weight score is used by our model to find which mail is spam
- min_df = 1 ;  so this is the basically that if the score of a particular word is less than 1 we need to ignore. If the score is greater than one then we can include it .
- the words we dont want like is ,the, did, etc these words are called as stop_words
