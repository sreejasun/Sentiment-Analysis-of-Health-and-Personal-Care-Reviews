The project involves sentiment analysis on Amazon review data using both traditional machine learning methods and pre-trained models from Hugging Face.

# Comprehensive Sentiment Analysis of Health and Personal Care Reviews Using Machine Learning and Pretrained Transformers
## 1. Machine Learning Apptoach
### Data Loading and Preprocessing:

**Loading Data:** Loading the data from a JSON file and examine its structure.
**Handling Missing Values:** There are no missing values in this dataset.
**Sentiment Labeling:** You convert ratings into sentiment labels (Negative, Neutral, Positive).

### Data Balancing:

Balance the dataset by downsampling the positive reviews and upsampling the neutral and negative reviews to ensure equal representation across sentiment categories.

### Text Preprocessing:

**Text Cleaning:** Removes HTML tags, punctuation, digits, and extra whitespace.
**Stop Words:** Custom set of stop words excluding some negative ones.
**Stemming:** Applies Porter Stemming to the words.

### Feature Extraction:

**Bag of Words:** Uses CountVectorizer to create a matrix of token counts.
**TF-IDF:** Uses TfidfVectorizer to represent text data based on term frequency-inverse document frequency.

### Model Training and Evaluation:

**Logistic Regression:** Trains and evaluates with various regularization parameters.
**Naive Bayes:** Trains and evaluates with different alpha values.
**Random Forest:** Trains and evaluates with different numbers of estimators.

### Model Predictions:

**Saved Models:** The trained models and vectorizers are saved using pickle.
**Prediction:** Uses saved models to predict sentiment for new reviews.


## 2. Using Hugging Face Pipeline:

**Pre-trained Model:** Uses a pre-trained sentiment analysis model from Hugging Face for predictions.


