# Procedure

## Purpose
- This repository reanalyses data from a _Science_ article by Tomasetti and Vogelstein, a pdf of which has been provided.
    - The article proposes that the lifetime risk of cancer is correlated with, among other factors, the total amount of stem cell divisions of a certain type of tissue.
- The overall purpose of this repository is to explore whether or not there is a correlation between total stem cell divisions and lifetime cancer risk in the provided data.
    - Hypothesis: the lifetime risk of cancer is correlated with the total amount of stem cell divisions of a certain type of tissue.
    - Null hypothesis: there is no correlation between the lifetime risk of cancer and total amount of stem cell divisions of a certain type of tissue.

## Data
- Data used here (Data.Log10LifetimeRisk.Log10TotaStemCellDivisions.txt) assessible from https://science.sciencemag.org/content/371/6535/1245?utm_campaign=toc_sci-mag_2021-03-18&et_rid=681382821&et_cid=3704890

## Data Analyses
- The steps used in this repository are as listed below
    - The cells and lines used for each step are provided in parenthesis.
1. Imported the pandas, numby, scipy, matplotlib.pyplot, pathlib, and sklearn libraries (cell 1, lines 1-6).
2. Imported data into a pandas DataFrame (cell 1, lines 8-12).
    - Dropped NaN values from dataframe (cell 1, lines 14-16).
3. Plotted both log-transformed values and raw values of lifetime cancer risk and total stem cell divisions in histograms (cells 2, 3, and 4).
    - This was done to determine whether raw values or log-transformed values better resembled a normal distribution.
        - For correlation tests, it is desirable that data resemble a normal distribution as closely as possible.
    - Extra statistics serving a similar purpose are provided in cell 5.
4. Plotted the data in a scatterplot and performed linear regression (cell 6, lines 1-17).
5. Calculated the coefficient of determination and slope of the linear regression model (cell 6, lines 19-20).
6. Calculated the R- and P-values of the linear regression model (cell 7).