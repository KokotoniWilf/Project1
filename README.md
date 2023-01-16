# UDACITY Data Scientist Nanodegree

## Project 1 - Writing a Data Science Blog Post


## Installations

This project requires Python 3.x and the following additional python libraries:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score, mean_squared_error
import seaborn as sns
import warnings
```

You will also require software that can run and execute an iPython Notebook


## Project Motivation

The aim of this project is to examine the Stack Overflow survey results for 2017 to attempt to answer the following questions:

1. How well can we predict an individual's career satisfaction?  What aspects correlate well to career satisfaction?
2. How does working remotely correlate with job and career satisfaction, and is there a correlation with salary?
3. Does the pronunciation of "GIF" differ between people who believe there is a right way and a wrong way to do everything and those who do not?



## File Descriptions

The files related to this project are as follows:

1. This README.md file, which contains information relating to the project aims and system requirements.
2. survey_results_public.csv - a csv file containing the survey results.  The dataset contains 51,392 responses.
3. Project_1_Code.ipynb - the python code used to answer the project questions.
4. survey_results_schema.csv - a csv file containing a description of each of the survey questions.  Not used in the analysis but included to provide clarity on the dataset columns should the viewer wish to learn more about them.

In addition there is a Medium blog post that presents the findings of this project.  The post can be found here.

## How to interact with the project

The code used to answer all 3 questions is held in Project_1_Code.ipynb.  This workbook should be opened and all code should be run.  Commentary and in-code comments are included in the notebook where appropriate.

## Results of Analysis

The detailed results analysis is included in the python notebook along with the code, and is also explained fully in the Medium blog post.  A brief summary for each question is noted below.

1. It was not possible to find a linear model that would provide accurate predictions of career satisfaction, with an r squared value of 0.41 for the test based on using 1131 columns.  Many of the main correlations were as one would expect (employment status, job satisfaction and how the respondents career had gone), however we were able to identify some intesting points such as working in Mexico having a positive correlation, but being paid in Mexican pesos having a negative correlation.
2. Working remotely appears to have a positive correlation with job satisfaction, career satisfaction and salary.  Never working remotely had the lowest mean values for all 3 of these categories, whilst working remotely all the time had the highest in all 3 categories.  Interestingly of those who worked remotely some but not all of the time, those who did it less than half the time scored higher than those wo did it half the time or more.
3. The more positively a respondant answered the premise "There is a right way and a wrong way to do everything", the less consistent their pronunciation of GIF was.  Those who strongly agreed with the premise were the most spread across the 4 possible answers suggesting that although this cohort believe there is a right way and a wrong way to do everything, they disagree on what that "right way" is.

## Licensing, Authors, Acknowledgements, etc

The dataset used in this analysis is provided by StackOverflow and is used in accordance with their licensing arrangement.
The dataset was hosted original on the Kaggle website.
