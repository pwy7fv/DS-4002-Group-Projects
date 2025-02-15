# Data Appendix

## Introduction/Overview:
The purpose of this data appendix is to provide a detailed description of the datasets analyzed, including relevant variables, summary statistics, and insights. This appendix includes two main datasets: one containing movie reviews from **June-July 2001** and another from **post-2011**. The movie reviews in both datasets correspond to the same movie, _The Fast and the Furious_, from the Fast and Furious franchise.

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
[Insert plot of reviews by date for June-July 2001]
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
- **Year Range**: 2001 for all
- **missing values**: None
- **method to final form**: The years were extracted from the full date using python

### Figures:
#### Figure 6: Distribution of Movie Reviews by Year (Post 2011)
![image](https://github.com/user-attachments/assets/a973f3ca-b073-49d5-a632-402fba468d42)
This graph shows how the average star rating changed over time

---



---

## Dataset  - 2 Fast 2 furious (Post 2013)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for _The Fast and the Furious_, written after **2011**. The unit of observation remains the same as in Dataset 1: a movie review with attributes such as Rating, Title, Content, Author Name, and Date.

### Variables:
- **Rating**: Numeric values representing the review rating, ranging from 1 to 10. Missing values were handled similarly as in the previous dataset by replacing "No rating" with the mean rating.
- **Title**: The name of the review.
- **Content**: The review text written by the user.
- **Author Name**: The name of the reviewer.
- **Date**: The date the review was posted.

### Descriptive Statistics:

#### Summary Statistics for Rating:
| Metric | Value |
|--------|-------|
| Count  | 208.000000 |
| Mean   |  6.240000 |
| Min    | 1.000000 |
| 25%    | 5.000000 |
| Median | 6.000000 |
| 75%    | 8.000000 |
| Max    | 10.000000  |
| Std Dev| 2.259152 |

#### Summary Statistics for Date:
- **Date Range**: [Insert the date range, e.g., from 2012 to 2023]
- **Total Number of Reviews**: [Insert total number of reviews]

#### Content:
- **Average Review Length**: [Insert calculated average review length here, e.g., number of characters]

#### Author Name:
- **Unique Reviewers**: [Insert number of unique authors]

#### Date:
- The reviews span from [Insert starting year, e.g., 2012] to the present.

---

### Figures and Tables:
#### Figure 2: Distribution of Movie Reviews by Date (Post-2011)

[Insert plot of reviews by date for post-2011]
---
## Conclusion:
This appendix provides an overview of two datasets, detailing the distribution of reviews, summary statistics, and key variables for both movie review periods. The data includes ratings, review content, and reviewer details, offering insights into public reception across different time periods. Further analysis of these reviews could reveal trends in user feedback and sentiment over time.

---

## Introduction/Overview:
The purpose of this data appendix is to provide a detailed description of the datasets analyzed, including relevant variables, summary statistics, and insights. This appendix includes two main datasets: one containing movie reviews from **June-July 2001** and another from **post-2011**. The movie reviews in both datasets correspond to the same movie, _The Fast and the Furious_, from the Fast and Furious franchise.

---

## Section 1: Dataset 1 - The Fast and Furious Reviews (June-July 2001)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for the first movie in the Fast and Furious franchise, _The Fast and Furious_, written between **June 22nd and July 13th, 2001**. The unit of observation is a movie review, where each row contains the following attributes:

### Variables:
- **Rating**: Numeric values representing the review rating. Missing data was replaced with the mean of all numeric ratings in the dataset.
- **Title**: The name of the review.
- **Content**: The review text written by the user.
- **Author Name**: The name of the reviewer.
- **Date**: The date the review was published.

### Descriptive Statistics:

#### Summary Statistics for Rating:
| Metric | Value |
|--------|-------|
| Count  | 321.000000|
| Mean   |  6.738318|
| Min    | 1.000000 |
| 25%    | 5.000000|
| Median | 7.000000|
| 75%    | 9.000000 |
| Max    | 10.000000 |
| Std Dev| 2.561749 |


#### Summary Statistics for Date:
- **Date Range**: 
- **Total Number of Reviews**: 162 ## check this 

#### Content:
- **Average Review Length**: [Insert calculated average review length here, e.g., number of characters] # need to calculate

#### Author Name:
- **Unique Reviewers**: [Insert number of unique authors] # need to calculate

#### Date:
- The reviews span from **June 22, 2001** to **July 13, 2001**.

---

### Figures and Tables:
#### Figure 1: Distribution of Movie Reviews by Date (June-July 2001)

[Insert plot of reviews by date for June-July 2001]
![image](https://github.com/user-attachments/assets/0359c083-ffa0-4205-8a11-b1e4ebee8010)

--

## Dataset  - The Fast and The Furious: Tokyo Drift (2006)

### Unit of Observation:
Each row in the dataset represents a movie review from a user for _The Fast and the Furious: Tokyo Drift_, written between June 16, 2006- July 6, 2006 and then post-2016. The unit of observation remains the same as in Dataset 1: a movie review with attributes such as Rating, Title, Content, Author Name, and Date.

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
| Count  | 103.000000 |
| Mean   | 6.071429 |
| Min    | 1.000000 |
| 25%    | 5.000000 |
| Median | 6.071429 |
| 75%    | 8.000000 |
| Max    | 10.000000  |
| Std Dev| 2.723613  |


#### Summary Statistics for Date:
- **Date Range**: June + July 2006 to 2016-2025
- **Total Number of Reviews**: [321 Total] [126 from June 16, 2006 - July 6, 2006] [195 from 2016-2025] 

#### Content:
- **Average Review Length**: [1059 Total] [1241 from June 16, 2006 - July 6, 2006] [942 from 2016-2025]

#### Author Name:
- **Unique Reviewers**: [320 Total] [126 from June 16, 2006 - July 6, 2006] [194 from 2016-2025]


#### Date:
- The reviews span from June 16, 2006 - July 6, 2006 to 2016 - 2025.


### Figures and Tables:
#### Distribution of The Fast and Furious: Tokyo Drift Movie Reviews by Date (June 16, 2006 - July 6, 2006 to 2016 - 2025.)
![image](https://github.com/user-attachments/assets/2b821d4a-bc01-4d67-a35c-c1f875e6c069)

--

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



