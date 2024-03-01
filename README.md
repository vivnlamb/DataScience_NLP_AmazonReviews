# NLP_PinkText_Analysis
Role: Team Lead, ideator and programmer for "Pink Text." 

https://www.canva.com/design/DAFhDrUMmPc/CstadgJD0bgw43kseo2T-w/view?utm_content=DAFhDrUMmPc&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink


Purpose: use sentimental analysis on pants marketed towards different genders. 

Organization: submitted to Samsung AI as Capstone Project.

## Project Phases:

## Part 1: Question

1. I proposed this project based on recent articles and viral media surrounding the lack of pockets in women's pants. I named the project "Pink Text," referencing the Pink Tax on women's products. 

## Part 2: Data Collection and Cleaning

AmazonApparel.ipynb

2. Finding the data: I used API to import an Amazon US Reviews dataset (now defunct) from Hugging Face to notebook
3. Challenge: could not find category for gender in dataset. Other public datasets have the same issue. Webscraping would take too much time and money.
4. **Solution: I used a novel approach, applying RegEx to extract the dataset necessary for this project, and wrote the final code for the final project submission.**
- genderless_pant_table: does not contain "women, men, boy, girl"
- gender_pant: contains "women, men"
- RegEx string: "(wo|m)(a|e)n|boy|girl"

5. Cleaning and preprocessing:
- “Bag of Words” used to divide indicator words for the classifier, a list of sentences joined as one string. All words lower cased, and stop words are removed.

6. Exploratory Data Analysis (EDA):
- The ratings for each dataset was graphed, showing interesting results. In these datasets, it was surprising that pants without gender in the product title had more high ratings and less low ratings than both men’s and women’s pants. Unsurprisingly, women’s pants had more low ratings and less high ratings than men’s pants.


## Part 3: Data Analysis, Modeling, and Visualization

7. NLTK Frequency Distribution was used to label each word with its count. The positive and negative word lists were combined into one set, then shuffled and split.
- I used Python’s Natural Language Toolkit (NLTK)
- I used NLTK frequency distribution to find the most common words, then the Naive Bayes classifier in the training and testing process, which allowed us to see the words most likely to lead to positive or negative classification in reviews.

## Results:
Naive Bayes was used to classify words in reviews as negative and positive, with a 70-80% accuracy across the three datasets (pants without gender, women’s pants, men’s pants). We intend to continue working on this project, with these improvements and further exploratory research concepts in mind:

Regression and predictive model for binary sentiment. Focus on Genderless Pants as a category for the market.
We can continue using sentiment analysis to predict if a review would be positive or negative, and build a predictive model. After the data has been classified by sentiment analysis, we can use logistic regression. We can convert text into numerical value, positive or negative, then use that as 0/1 value as predictor. The model will take the numerically expressed features as input, and the output is predicted binary sentiment.

The Genderless Pants also have more High Ratings and less Low Ratings than BOTH Men's Pants and Women's pants, so we can continue to find features in the Amazon Reviews to expand this product as a category for NonBinary customers.

## Next Step:

Now that ChatGPT made "traditional" NLP data modeling methods like the one I used outdated overnight, I plan to apply Large Language Models to the same dataset, and compare the results.


