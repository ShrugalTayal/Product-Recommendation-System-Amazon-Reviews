# CSE508_Winter2024_A3_2020408
 
## Product Recommendation System based on Amazon Review

### Author: 
ShrugalTayal (shrugal20408@iiitd.ac.in)

### Introduction
The Product Recommendation System based on Amazon Review aims to predict user ratings and provide personalized recommendations for electronics products. Leveraging collaborative filtering techniques, the system analyzes user interactions and preferences to suggest the most relevant items.

### Dataset
The dataset used for this project is the Amazon Reviews Dataset, specifically the 5-core dataset for the Electronics category, available from Amazon. The dataset contains reviews and metadata for various electronics products.

### Steps:

#### 1. Data Loading and Preprocessing
- Load the dataset into a dataframe.
- Perform preprocessing steps such as handling missing values, duplicates, and other data cleaning tasks.

#### 2. Descriptive Statistics
- Report the total number of reviews, average rating score, and other descriptive statistics for the chosen product (e.g., Headphones).

#### 3. Text Preprocessing
- Remove HTML tags, accented characters, and special characters.
- Expand acronyms and perform lemmatization to normalize the text.

#### 4. Exploratory Data Analysis (EDA)
- Identify the top and least reviewed brands in the chosen category.
- Determine the most positively reviewed product.
- Analyze the distribution of ratings over consecutive years.
- Create word clouds for good and bad ratings to identify common positive and negative words.
- Plot a pie chart showing the distribution of ratings vs. the number of reviews.
- Identify the year with the maximum reviews and the highest number of customers.

#### 5. Feature Engineering
- Use Bag of Words model, TF-IDF, Hashing Vectorizer, or Word2Vec to model review text as features.

#### 6. Machine Learning Models
- Divide the data into training and testing sets.
- Use the review text as the input feature and the rating class as the target variable.
- Compare the performance of five machine learning models based on precision, recall, F-1 score, and support for each target class.

#### 7. Collaborative Filtering
- Create a user-item rating matrix.
- Normalize the ratings using min-max scaling.
- Build a user-user recommender system:
  - Find the top N similar users using cosine similarity.
  - Use K-folds validation to predict missing values and calculate errors.
  - Report the Mean Absolute Error (MAE) for different values of N.
- Implement an item-item recommender system following similar steps as the user-user system.
- Plot graphs showing MAE against N for both recommender systems.

#### 8. Top Products by User Sum Ratings
- Report the top 10 products based on user sum ratings.

### Conclusion
The Product Recommendation System based on Amazon Review leverages data analysis and machine learning techniques to provide personalized recommendations for electronics products. By understanding user preferences and behavior, the system enhances user engagement and satisfaction.