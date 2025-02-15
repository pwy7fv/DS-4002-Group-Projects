# Data Appendix

## Introduction/Overview:

---

## Section 1: Dataset 1 - The Fast and Furious Reviews (June-July 2001)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for the first movie in the Fast and Furious franchise, _The Fast and Furious_, written between **June 22nd and July 13th, 2001**. The unit of observation is a movie review, where each row contains the following attributes:

### Variables:
- **Rating**: Floats 
- **Title**: Objects
- **Content**: Object
- **Author Name**: Object
- **Date**: DateTime 
- **Year**: Float
 

### Descriptive Statistics:

#### Summary Statistics for Rating:
- **Defintion**: Numeric values representing the review rating. Missing data was replaced with the mean of all numeric ratings in the dataset.
- **missing values**: There are no missing values in the datset after cleaning, they were replaced by the mean rating score of the datset
- **method to final form**: The dates were extracted from the movie's IMDb page using Selenium. In Python, the mean for the specified time period was calculated and used to replace any "No rating" values in the dataset.

### Figures and Tables:

| Metric | Value |
|--------|-------|
| Count  | 162   |
| Mean   | 7.93  |
| Min    | 1     |
| 25%    | 7.93  |
| Median | 8     |
| 75%    | 10    |
| Max    | 10    |
| Std Dev| 2.29  |

#### Figure 1:  Boxplot of data (June-July 2001)
![image](https://github.com/user-attachments/assets/44b45ace-5115-47e1-85db-6e3f1347e4af)
*The June-July 2001 dataset consists of 162 reviews with an average rating of 7.93. Ratings range from 1 to 10, with most ratings being above 7.93. The median rating is 8, and the standard deviation is 2.29, indicating some variation in user opinions. Most reviews are highly positive, with a significant number of 10 ratings.*

#### Figure 2: Mean of Movie Reviews by Date (June-July 2001)
![image](https://github.com/user-attachments/assets/8b2436f8-4d4c-4a6d-af68-9728808a11b2)
This graph shows how the average star rating changes over time


#### Summary Statistics for Date:
- **Defintion**: The date the review was published.
- **Date Range**: The reviews span from **June 22, 2001** to **July 13, 2001**.
- **missing values**: None
- **method to final form**: The dates were scraped from the movies imdb page using selenium. It was then changed to fit a YYYY-MM-DD format in python. 

### Figures:
#### Figure 3: Distribution of Movie Reviews by Date (June-July 2001)
![image](https://github.com/user-attachments/assets/6ecaaa95-3d24-4395-8de6-c533e4a3f873)
This graph shows the distribution of reivew dates

#### Summary of Title:
- **Defintion**: The name of the review.
- **missing values**: None
- **method to final form**: The review titles were scraped from the movies imdb page using selenium.
  
#### Summary of Content:
**Defintion**: The review text written by the user.
- **missing values**: None
- **method to final form**: Reviews were scraped from the movie’s IMDb page using Selenium. Reviews marked with a spoiler warning were initially scraped as having "No content". To clean the dataset, missing reviews were manually identified, and content was copied from the original source into the CSV file.


#### Summary of Author Name:
- **Definition**: The name of the reviewer
- **missing values**: None
- **method to final form**: The reviewers names were scraped from the movies imdb page using selenium.

#### Summary of Year:
- **Defintion**: The Year the review was published.
- **Year Range**: 2001 for all
- **missing values**: None
- **method to final form**: The years were extracted from the full date using python
---

## Section 2: Dataset 2 - The Fast and Furious Reviews (Post-2011)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for _The Fast and the Furious_, written during and after **2011**. The unit of observation remains the same as in Dataset 1: a movie review with attributes such as Rating, Title, Content, Author Name, and Date.

### Variables:
- **Rating**: Floats 
- **Title**: Objects
- **Content**: Object
- **Author Name**: Object
- **Date**: DateTime 
- **Year**: Float

### Descriptive Statistics:

#### Summary Statistics for Rating:
- **Defintion**: Numeric values representing the review rating. Missing data was replaced with the mean of all numeric ratings in the dataset.
- **missing values**: There are no missing values in the datset after cleaning, they were replaced by the mean rating score of the datset
- **method to final form**: The dates were extracted from the movie's IMDb page using Selenium. In Python, the mean for the specified time period was calculated and used to replace any "No rating" values in the dataset.
### Figures and Tables:
| Metric | Value |
|--------|-------|
| Count  | 374.000000|
| Mean   | 7.442308 |
| Min    | 1.000000 |
| 25%    | 6.000000 |
| Median | 8.000000 |
| 75%    | 10.000000|
| Max    | 10.000000 |
| Std Dev| 2.34765|

#### Figure 4:  Boxplot of data (2011 and after)
![image](https://github.com/user-attachments/assets/58a0b7e0-607c-4535-814b-9177bcc1d54b)
*This dataset contains 374 reviews, with ratings ranging from 1 to 10. The average rating is 7.44, and the ratings are generally distributed between 6 and 10. The reviews span from April 28, 2011, to February 3, 2025, with a notable concentration of reviews around 2021 and 2023. The standard deviation of ratings is 2.35, indicating moderate variability in user reviews.*

#### Figure 5: Mean of Movie Reviews by Date (2011 and after)
![image](https://github.com/user-attachments/assets/2d44648a-4cc9-4ca5-b828-56d55394d032)
This graph shows the distribution of reviews by year

#### Summary Statistics for Date:
- **Defintion**: The date the review was published.
- **Date Range**: - The reviews include anything posted on IMdb after Dec 31, 2010

#### Summary of Title:
- **Defintion**: The name of the review.
- **missing values**: None
- **method to final form**: The review titles were scraped from the movies imdb page using selenium.
  
#### Summary of Content:
**Defintion**: The review text written by the user.
- **missing values**: None
- **method to final form**: Reviews were scraped from the movie’s IMDb page using Selenium. Reviews marked with a spoiler warning were initially scraped as having "No content". To clean the dataset, missing reviews were manually identified, and content was copied from the original source into the CSV file.

#### Summary of Author Name:
- **Definition**: The name of the reviewer
- **missing values**: None
- **method to final form**: The reviewers names were scraped from the movies imdb page using selenium.

#### Summary of Year:
- **Defintion**: The Year the review was published.
- **Year Range**: 20011 - 2025
- **missing values**: None
- **method to final form**: The years were extracted from the full date using python

### Figures:
#### Figure 6: Distribution of Movie Reviews by Year (Post 2011)
![image](https://github.com/user-attachments/assets/a973f3ca-b073-49d5-a632-402fba468d42)
This graph shows how the average star rating changed over time

---

## Section 3: Dataset 3 - 2 Fast 2 Furious Reviews (June 2003)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for the second movie in the Fast and Furious franchise, _2 Fast 2 Furious_, written between **June 6th 2003 and June 28th, 2003**. The unit of observation is a movie review, where each row contains the following attributes:

### Variables:
- **Rating**: Floats 
- **Title**: Objects
- **Content**: Object
- **Author Name**: Object
- **Date**: DateTime 
- **Year**: Float
 
### Descriptive Statistics:

#### Summary Statistics for Rating:
- **Defintion**: Numeric values representing the review rating. Missing data was replaced with the mean of all numeric ratings in the dataset.
- **missing values**: There are no missing values in the datset after cleaning, they were replaced by the mean rating score of the datset
- **method to final form**: The dates were extracted from the movie's IMDb page using Selenium. In Python, the mean for the specified time period was calculated and used to replace any "No rating" values in the dataset.

### Figures and Tables:

| Metric   | Value    |
|----------|----------|
| Count    | 103  |
| Mean     | 6.07    |
| Min      | 1   |
| 25%      | 5  |
| Median   | 6.07   |
| 75%      | 8  |
| Max      | 10    |
| Std Dev  | 2.72  |

#### Figure 1:  Boxplot of data (June 2003)
![image](https://github.com/user-attachments/assets/3cc066e1-9b79-49ef-82e5-c7bbe5c1f009)
*This boxplot displays the distribution of ratings for the movie reviews in June 2003. The ratings range from 1 to 10, with a median rating of 6.07 and a mean of 6.07. The dataset consists of 103 reviews, and the ratings show a moderate spread, with a standard deviation of 2.72.


#### Figure 2: Mean of Movie Reviews by Date (June 2001)
![image](https://github.com/user-attachments/assets/e1b608f8-4f3d-4ce2-ab11-6cba3e16d408)
This graph shows how the average star rating changes over time


#### Summary Statistics for Date:
- **Defintion**: The date the review was published.
- **Date Range**: The reviews span from **June 6, 2003** to **July 28, 2003**.
- **missing values**: None
- **method to final form**: The dates were scraped from the movies imdb page using selenium. It was then changed to fit a YYYY-MM-DD format in python. 

### Figures:
#### Figure 3: Distribution of Movie Reviews by Date (June 2003)
![image](https://github.com/user-attachments/assets/eb28c1c9-e49d-45c0-a8bf-fe46e3a7d56f)

This graph shows the distribution of reivew dates

#### Summary of Title:
- **Defintion**: The name of the review.
- **missing values**: None
- **method to final form**: The review titles were scraped from the movies imdb page using selenium.
  
#### Summary of Content:
**Defintion**: The review text written by the user.
- **missing values**: None
- **method to final form**: Reviews were scraped from the movie’s IMDb page using Selenium. Reviews marked with a spoiler warning were initially scraped as having "No content". To clean the dataset, missing reviews were manually identified, and content was copied from the original source into the CSV file.

#### Summary of Author Name:
- **Definition**: The name of the reviewer
- **missing values**: None
- **method to final form**: The reviewers names were scraped from the movies imdb page using selenium.

#### Summary of Year:
- **Defintion**: The Year the review was published.
- **Year Range**: 2003 for all
- **missing values**: None
- **method to final form**: The years were extracted from the full date using python
---

## Section 4: Dataset 4 - 2 Fast 2 Furious Reviews (2013 and after)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for _2 Fast to Furious, written after **2013**. The unit of observation remains the same as in Dataset 1: a movie review with attributes such as Rating, Title, Content, Author Name, and Date.

### Variables:
- **Rating**: Floats 
- **Title**: Objects
- **Content**: Object
- **Author Name**: Object
- **Date**: DateTime 
- **Year**: Float
 
### Descriptive Statistics:

#### Summary Statistics for Rating:
- **Defintion**: Numeric values representing the review rating. Missing data was replaced with the mean of all numeric ratings in the dataset.
- **missing values**: There are no missing values in the datset after cleaning, they were replaced by the mean rating score of the datset
- **method to final form**: The dates were extracted from the movie's IMDb page using Selenium. In Python, the mean for the specified time period was calculated and used to replace any "No rating" values in the dataset.
  
#### Summary Statistics for Rating:

| Metric   | Value    |
|----------|----------|
| Count    | 208      |
| Mean     | 6.24     |
| Min      | 1.00     |
| 25%      | 5.00     |
| Median   | 6.00     |
| 75%      | 8.00     |
| Max      | 10.00    |
| Std Dev  | 2.26     |
`

#### Figure 1:  Boxplot of data (2013 and after)
![image](https://github.com/user-attachments/assets/ea807096-9269-4016-85bd-bf0ed44e8cb6)
*The boxplot above displays the distribution of ratings for the Post-2013 Fast and Furious dataset. The median rating is around 6, with a wide range of reviews, from 1 to 10. The distribution has a similar shape to the 2003 dataset.


#### Figure 2: Mean of Movie Reviews by Date (2013 and after)
![image](https://github.com/user-attachments/assets/2b41cadf-c14e-4c6a-9c58-10fa3e99b969)
This graph shows how the average star rating changes over time


#### Summary Statistics for Date:
- **Defintion**: The date the review was published.
- **Date Range**: The reviews span from **February 14, 2013** to **ebruary 4, 2025**.
- **missing values**: None
- **method to final form**: The dates were scraped from the movies imdb page using selenium. It was then changed to fit a YYYY-MM-DD format in python. 

#### Summary of Content:
**Defintion**: The review text written by the user.
- **missing values**: None
- **method to final form**: Reviews were scraped from the movie’s IMDb page using Selenium. Reviews marked with a spoiler warning were initially scraped as having "No content". To clean the dataset, missing reviews were manually identified, and content was copied from the original source into the CSV file.

#### Summary of Author Name:
- **Definition**: The name of the reviewer
- **missing values**: None
- **method to final form**: The reviewers names were scraped from the movies imdb page using selenium.

#### Summary of Year:
- **Defintion**: The Year the review was published.
- **Year Range**: 2013-2025
- **missing values**: None
- **method to final form**: The years were extracted from the full date using python
### Figures:
#### Figure 3: Distribution of Movie Reviews by Year (2013 and after)
![image](https://github.com/user-attachments/assets/9404e9fe-fafe-482f-8431-3d47fb957b13)

---


## Dataset  - Fast & Furious (2009)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for _The Fast and the Furious: Tokyo Drift_, written between March 30, 2009- April 9, 2009 and then post-2019. The unit of observation remains the same as in Dataset 1: a movie review with attributes such as Rating, Title, Content, Author Name, and Date.

### Variables:
- **Rating**: Numeric values representing the review rating, ranging from 1 to 10. Missing values were handled similarly as in the previous dataset by replacing "No rating" with the mean rating.
- **Title**: The name of the review.
- **Content**: The review text written by the user. Missing text was handled by manually finding the mising text from IMDb wesbite and adding them to the dataframe.
- **Author Name**: The name of the reviewer.
- **Date**: The date the review was posted.

### Descriptive Statistics:

#### Summary Statistics for Rating:
| Metric | Value |
|--------|-------|
| Count  | |180.000000|
| Mean   |  6.677778|
| Min    | 1.000000 |
| 25%    | 6.000000 |
| Median | 6.677777777777778|
| 75%    | 8.000000|
| Max    |  10.000000 |
| Std Dev|  2.043263 |


#### Summary Statistics for Date:
- **Date Range**: March 2009 to 2019-2025
- **Total Number of Reviews**: [180 Total] [66 from March, 30 2009 - April, 9 2009] [114 from 2016-2025] 

#### Content:
- **Average Review Length**: [1114 Total] [1384 from June 16, 2006 - July 6, 2006] [959 from 2016-2025]

#### Author Name:
- **Unique Reviewers**: [180 Total] [66 from June 16, 2006 - July 6, 2006] [114 from 2016-2025]


#### Date:
- The reviews span from March 30, 2009 - April 9, 2009 to 2019 - 2025.


### Figures and Tables:
#### Distribution of Fast & Furious Movie Reviews by Date (March 30, 2009 - April 9, 2009 to 2019 - 2025)
![image](https://github.com/user-attachments/assets/a2da0df7-54ca-4dd7-9c1e-f935b1c5aa13)



