
# Movies and Money
 
**Author:** Melvin Gonzalez, Jr. \
**Dataset Source:** [TMDb Database](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## Project Overview

This project explores key factors that influence the financial success of movies in Hollywood. By analyzing data from the TMDb database, I aim to answer the question: **What traits and characteristics of movies lead to higher box office returns and ROI?** The analysis focuses on features that producers can influence (like genres, budgets, and release years) rather than factors outside of their control (e.g., TMDb votes).

The project includes data cleaning, exploratory data analysis (EDA), feature engineering, and insights into trends over time. It showcases the potential of data analysis to guide decision-making in the movie industry, identifying what elements may contribute to higher revenue and profitability.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Wrangling](#data-wrangling)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Conclusions](#conclusions)
5. [Future Work](#future-work)
6. [Technologies Used](#technologies-used)

## Introduction

In this project, I analyzed a subset of the TMDb movie dataset to explore trends in movie revenue and return on investment (ROI). I focused on variables that Hollywood producers can control—such as genre, budget, and release year—while analyzing revenue trends across time.

The main objective is to determine what factors might lead to a higher box office return and what has contributed to Hollywood's most successful movies over the years.

## Data Wrangling

The dataset required extensive cleaning to be usable for analysis. Key steps include:

- **Dropping irrelevant columns**: Removed columns with over 10% missing data and those outside a producer’s control (e.g., popularity, votes).
- **Handling missing data**: Removed rows with missing `revenue_adj`, the target variable.
- **Outlier treatment**: Excluded movies with implausibly low budgets and revenues (e.g., films with a budget of a few cents).
- **Feature engineering**: Created a **ROI** column (`revenue_adj/budget_adj`) to analyze the return on investment of each movie.

## Exploratory Data Analysis

Key analyses performed include:

- **Revenue and ROI over time**: Plotted how movie revenues and ROI have changed from the 1970s to the present day, showing a downward trend after a peak in the 1970s.
- **Genre trends**: Analyzed the popularity of movie genres in the 1970s compared to today. Drama, Action, Thriller, and Adventure (D.A.T.A.) were the most popular genres in the 70s.
- **Histograms and line plots**: Explored the distribution of revenues and trends in movie production volume over the years.

## Key Insights

1. **Revenue and ROI have declined** over the years since their peak in the 1970s. Despite larger overall box office numbers, the average movie has become less profitable when adjusted for inflation.
2. **Genres**: While the most popular genres from the 1970s remain relevant, they do not show a clear correlation with higher revenues in later decades. Other factors likely play a significant role in a movie’s financial success.
3. **Budget thresholds**: Movies with an adjusted budget of over $100K seem to show more stable trends in both revenue and ROI, while those below this threshold often skew results.

## Conclusions

This analysis provides initial insights into what traits could influence the box office performance of a movie, particularly for Hollywood producers. However, further analysis is necessary to establish more definitive relationships between factors like genre, actors, and budget with financial success. 

Despite finding no strong correlation between genres and revenue, this project has opened up more avenues for future analysis, particularly in exploring additional features like actor/director influence and the effect of release dates or marketing campaigns.

## Future Work

There are several ways this project could be extended:

- **Machine Learning**: Implement predictive models (e.g., linear regression) to forecast a movie’s potential revenue based on features like budget, genre, and cast.
- **Sentiment Analysis**: Use natural language processing (NLP) on movie reviews to see if sentiment scores influence a movie’s success.
- **Clustering**: Use clustering algorithms to identify different classes of movies (e.g., blockbusters vs. independent films) based on budget, revenue, and ROI.
- **Actor/Director Influence**: Add features for actor and director popularity to explore how the creative team impacts box office performance.

## Technologies Used

- **Python**: Main language used for analysis.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Matplotlib** & **Seaborn**: For data visualization.
- **Jupyter Notebook**: Environment for exploratory analysis.

## How to Run

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/movies_and_money.git
   ```
2. Install the required packages:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook `movies_and_money.ipynb` to view the analysis or execute it on your local machine.

## Contact

If you have any questions or suggestions, feel free to reach out at mgonzalez713@gmail.com or connect with me on [LinkedIn](https://www.linkedin.com/in/melvingonzalezjr). As a student learning more about Data Science and AI, I'm open to opportunities to learn and grow! :)


