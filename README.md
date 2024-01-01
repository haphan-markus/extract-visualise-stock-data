# Extracting and visualising stock data

# Description
This project applies Python in Jupyter Notebook to extract the revenue data for Tesla and Gamestop and build a dashboard to compare the price of the stock and the revenue.

# Usage

Please refer to the Jupyter Notebook "Final project.ipynb" in the repo.

# Library

The project utilises Python libraries:
    * Pandas
    * yfinance
    * requests
    * Beautiful Soup
    * plotly
    * warnings

These libraries need to be installed in the working environment before running the Jupyter Notebook, using Terminal or command prompt.

# Visualisation

    * Extracting Tesla Stock Data Using yfinance

![Alt text](./assets/screenshots/image1.png)

![Alt text](./assets/screenshots/image2.png)

The `teslaData` Dataframe originally consists of 3400 rows with 7 columns.

![Alt text](./assets/screenshots/image3.png)

**Reset the index** using the `reset_index(inplace=True)` function on the tesla_data DataFrame and display the first five rows of the `teslaData` dataframe using the `head` function. Take a screenshot of the results and code from the beginning of Question 1 to the results below.

![Alt text](./assets/screenshots/image4.png)