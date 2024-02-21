# NLP_PinkText_Analysis
Role: Team Lead, ideator and programmer for "Pink Text." 

Purpose: use sentimental analysis on pants marketed towards different genders. 

Organization: submitted to Samsung AI as Capstone Project.

Project Phases:

1. I proposed this project based on recent articles and viral media surrounding the lack of pockets in women's pants. I named the project "Pink Text," referencing the Pink Tax on women's products. 

AmazonApparel.ipynb
2. Finding the data: I used API to import an Amazon US Reviews dataset (now defunct) from Hugging Face to notebook
3. Challenge: could not find category for gender in dataset. Other public datasets have the same issue. Webscraping would take too much time and money.
- Solution: I used a novel approach, applying RegEx to extract the dataset necessary for this project, and wrote the final code for the final project submission.

4. I used Naive Bayes Classifier and applied it to genderless pants to find features associated with positive and negative ratings in Amazon reviews for Women’s and Men’s pants.
5. I used different visualization methods, e.g. word cloud, to summarize results for non-technical audiences.
6. I provided the results to my team, and we created a list of actionable insights for product improvements and marketing around pants and gender.
