# DS-4002-Group-Projects : TEAM SBT

## Section 1: Software and Platform Used

### Software:
- **Python**: The primary programming language used for this project.
- **PyCharm**: The Integrated Development Environment (IDE) used for coding, specifically for sentiment analysis with VADER.
- **Google Colab**: The cloud-based platform used for running Jupyter notebooks, particularly for data analysis, cleaning, and visualization.
  
### Add-on Packages:
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Matplotlib** and **Seaborn**: For data visualization, including histograms and box plots.
- **Requests**: For making HTTP requests to retrieve web content.
- **Selenium**: For web scraping, particularly for scraping data from IMDb.
- **Chromium and Chromedriver**: Used in conjunction with Selenium to control the web browser for scraping.
- **BeautifulSoup**: For parsing HTML content to extract specific data.
- **VADER** (via `vaderSentiment`): For performing sentiment analysis on the reviews.

### Platform:
- **Mac** and **Windows**: These operating systems were used during development.
- **Google Colab**: Used as an online platform to execute Python code and visualize data in real-time.


### Map of Documentation

**DS-4002-GROUP-PROJECTS**
- DATA (main folder)
    - Cleaned Data (sub folder)
        - FAF1_2001_cleaned.csv
        - FAF1_2011_cleaned.csv
        - FAF1_2013_cleaned.csv
        - FAF1_2003_cleaned.csv
        - FF3_clean_data.csv
        - FF4_clean_data.csv
        - FF5_clean_dec2.csv
        - FF5_clean2011_3.csv
        - FF6_clean_dec2.csv
        - FF6_clean2013_2.csv
    - Original Data (sub folder)
        - FF2reviews_data.csv
        - FF3reviews_data.csv
        - FF4reviews_data.csv
        - FF5reviews_data.csv
        - FF6reviews_data.csv
        - reviews_data(1).csv
        - reviews_data.csv
    - Data_Appendix.md
    - image-1.png (graph in data appendix)
    - image-2.png (graph in data appendix)
    - image-3.png (graph in data appendix)
    - image-4.png (graph in data appendix)
    - image-5.png (graph in data appendix)
    - image-6.png (graph in data appendix)
    - image-7.png (graph in data appendix)
    - image.png (graph in data appendix)
- OUTPUT (main folder)
    - FF3_ + FF4_Vader_Visualizations.ipynb
    - FF3_Vader_Analysis.ipynb
- SCRIPTS (main folder)
    - DS-4002-Group-Projects
    - Cleaning_FAF1_FAF2_PLUS_GRAPHING.ipynb
    - FF3_ + FF4_clean.ipynb
    - FF5_clean.ipynb
    - FF6_clean.ipynb
    - Selenium_Dynamic_Scraping.ipynb
- delete.md
- LICENSE.md
- README.md




## A Map of your documentation.
In the folder DATA, The reviews for each movie beofre and after
In the OUTCOME FOLDER .... I assume is graphs and styff
In the Scripts folder is the coding performed

## Instructions for reproducing your results. 
Scraping

We first scraped data from IMDb user movie reviews for the first six movies in the Fast and Furious franchise. We used Selenium and BeautifulSoup4 to perform the scraping. Selenium was essential for handling dynamic scraping, which meant dealing with multiple pages of reviews rather than just the first page.

To accomplish this, we accessed the page source of the IMDb user review section for each movie and identified the class types for different pieces of data. We scraped the following information: Rating, Author Name, Title of Review, Content of Review, and Date. Additionally, we had to locate the class type for the "ALL" button to extract all available reviews rather than just the first 25 that appeared by default.

A few important considerations:

- Any reviews containing spoilers were blocked by IMDb and could not be scraped. These were labeled as "No content" so we could manually add them later.
- Any ratings that failed to scrape properly were marked as "No rating."
- The complete code and step-by-step process for dynamic scraping can be found in the Scripts folder under the file labeled "Selenium_Dynamic_Scraping."

Cleaning

After scraping, we proceeded with cleaning the data. Each team member was responsible for two movies. The cleaning code is stored in the Scripts folder, with a separate file for each movie.

Key steps in data cleaning:

Data Type Conversion:
- The Date column was converted to datetime.
- The Rating column was converted to float.
- Other columns remained as objects.

Adding a "Year" Column:
- We created a new column, "Year," and converted it to an integer format.
- This made it easier to analyze both numerical and categorical variables.

Filtering for Relevant Years:
- We included reviews from a maximum of one month after each movie’s release date and a decade later to the present.
- For example, for the first movie (released in 2001), we gathered reviews up to one month post-release and then from 2011 to the present.
- This allowed us to compare audience reactions shortly after release with opinions a decade later.

Handling Missing Data:
- "No rating" entries were replaced with the mean rating from the successfully scraped data.
- "No content" entries were manually updated by retrieving the missing text from IMDb user reviews. This was done using either a dictionary in Python or manually in Excel.

Finally, the cleaned dataset was saved as a CSV file and uploaded to the Scripts folder.

Analysis with VADER

Once the data was cleaned, we applied the VADER Sentiment Analysis tool to evaluate the sentiment of the reviews. We then added this newly found information as columns to our datasets. This new data from VADER consisted of:

- The percentage of positive sentiments in each review reviews which was named "Positive Score." 
- The percentage of neutral sentiments in each reviews which was named "Neutral Score."
- The percentage of negative sentiments in each review which was named "Negative Score."
- An overall sentiment percentage determining whether a review was mostly positive, neutral, or negative, which was named "Overall Percenteange Score."
- An overal sentiment lable of positve, neutral , or negative, which was named "Overall Sentiment"
As part of our analysis, we generated many visualizations comparing the two different time periods for each movie in the franchise. 

All analysis outputs, including sentiment results and visualizations, can be found in the OUTPUT folder. Each file is named according to the corresponding movie. So for example the Fast & Furious (2009) and fourth in the franchishe is called FF4.  

--

## Section 4: References!
[1] Ansari, Aamir Ahmad. “Selenium with Beautifulsoup Tutorial[Python].” Medium, 17 Jan. 2022. [Online]. 
Available: aamir07.medium.com/selenium-with-beautifulsoup-tutorial-python-ff9362e1571c. [Accessed: Feb. 5, 2025].

[2] ChatGPT, “Chatgpt.” [Online]. Available: chatgpt.com/. [Accessed 5 Feb. 2025].

[3] GeeksforGeeks “How to Conduct a Two Sample T-Test in Python.” GeeksforGeeks, 17 Oct. 2022. [Online].
Available: www.geeksforgeeks.org/how-to-conduct-a-two-sample-t-test-in-python/. [Accessed: Feb 15, 2025].

[4] Gong, Jason. “Web Scraping Rotten Tomatoes: A Step-by-Step Guide.” Bardeen AI: Workflow Task Automation Software, 3 Mar. 2024. [Online]. Available: www.bardeen.ai/answers/how-to-web-scrape-rotten-tomatoes. [Accessed: Feb. 5, 2025].

[5] Hutto, C.J. “VADER-Sentiment-Analysis.” GitHub, 14 Mar. 2021. [Online]. 
Available: github.com/cjhutto/vaderSentiment. [Accessed: Feb. 2, 2025].

[6] IMDb, “The Fast and the Furious User Reviews,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt0232500/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[7] IMDb, “2 Fast 2 Furious User Reviews,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt0322259/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[8] IMDb, “The Fast and the Furious: Tokyo Drift User Reviews ,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt0463985/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[9] IMDb, “Fast & Furious User Reviews ,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt1013752/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[10] IMDb, “Fast Five User Reviews ,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt1596343/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[11] IMDb, “Fast & Furious 6 User Reviews ,” IMDb. [Online]. 
Available: https://www.imdb.com/title/tt1905041/reviews/?ref_=tt_ururv_sm. [Accessed: Feb. 3, 2025].

[12] Nayak, Rahul. “Web Scraping Using Beautiful Soup and Selenium for Dynamic Page.” Medium, YML Innovation Lab. 16 Feb. 2019. [Online].
Available: medium.com/ymedialabs-innovation/web-scraping-using-beautiful-soup-and-selenium-for-dynamic-page-2f8ad15efe25.
[Accessed: Feb. 5, 2025].

[13] “Sentiment Analysis Using Vader - Using Python.” GeeksforGeeks, 11 Dec. 2024. [Online].
Available: www.geeksforgeeks.org/python-sentiment-analysis-using-vader/. [Accessed: Feb. 4, 2025].

[14] Sreedar, Arjhun. “Running Selenium on Google Colab.” Medium, 31 Oct. 2023. [Online].
Available: medium.com/@MinatoNamikaze02/running-selenium-on-google-colab-a118d10ca5f8. [Accessed: Feb. 5, 2025].

[15] ThetaTheta. “How to Save the Result of Scraping in a CSV?” Stack Overflow, 2 Sept. 2021. [Online]. 
Available: stackoverflow.com/questions/69030056/how-to-save-the-result-of-scraping-in-a-csv. [Accessed: Feb. 5, 2025].

[16] Yoo, Nari. “[Python] How to Run Selenium in Google Colab.” Nari’s Research Log, 21 June 2023.[Online].
Available: nariyoo.com/python-how-to-run-selenium-in-google-colab/. [Accessed: Feb. 5, 2025].

