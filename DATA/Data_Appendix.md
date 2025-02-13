# Data Appendix

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
| Count  | 162   |
| Mean   | 7.93  |
| Min    | 1     |
| 25%    | 7.93  |
| Median | 8     |
| 75%    | 10    |
| Max    | 10    |
| Std Dev| 2.29  |

#### Summary Statistics for Date:
- **Date Range**: June 22, 2001 - July 13, 2001
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


---

## Section 2: Dataset 2 - The Fast and Furious Reviews (Post-2011)

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
| Count  | [Insert count] |
| Mean   | [Insert mean] |
| Min    | [Insert min rating] |
| 25%    | [Insert 25th percentile] |
| Median | [Insert median] |
| 75%    | [Insert 75th percentile] |
| Max    | [Insert max rating] |
| Std Dev| [Insert standard deviation] |

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
