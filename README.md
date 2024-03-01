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

## Part 3: Data Analysis and Visualization

5. I used Naive Bayes Classifier and applied it to genderless pants to find features associated with positive and negative ratings in Amazon reviews for Women’s and Men’s pants.
6. I used different visualization methods, e.g. word cloud, to summarize results for non-technical audiences.
7. I provided the results to my team, and we created a list of actionable insights for product improvements and marketing around pants and gender.
