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

# Tesla stock and revenue dashboard

    1. Extracting Tesla Stock Data Using yfinance

![Alt text](./assets/screenshots/image1.png)

![Alt text](./assets/screenshots/image2.png)

The `teslaData` Dataframe originally consists of 3400 rows with 7 columns.

![Alt text](./assets/screenshots/image3.png)

**Reset the index** using the `reset_index(inplace=True)` function on the tesla_data DataFrame and display the first five rows of the `teslaData` dataframe using the `head` function.

![Alt text](./assets/screenshots/image4.png)

    2. Extracting Tesla Revenue Data Using Webscraping

![Alt text](./assets/screenshots/image5.png)

Using `BeautifulSoup` or the `read_html` function extract the table with `Tesla Revenue` and store it into a dataframe named `tesla_revenue`. The dataframe should have columns `Date` and `Revenue`.

![Alt text](./assets/screenshots/image6.png)

Remove the comma and dollar sign from the `Revenue` column. 

![Alt text](./assets/screenshots/image7.png)

Remove an null or empty strings in the `Revenue` column.

![Alt text](./assets/screenshots/image8.png)

Display the last 5 row of the `tesla_revenue` dataframe using the `tail` function.

![Alt text](./assets/screenshots/image9.png)

    3. Tesla dashboard

![Alt text](./assets/screenshots/image10.png)

# Gamestop stock and revenue dashboard

    1. Extracting Gamestop Stock Data using yfinance

Using the `Ticker` function enter the ticker symbol of the stock we want to extract data on to create a ticker object. The stock is GameStop and its ticker symbol is `GME`.

![Alt text](./assets/screenshots/image11.png)

Using the ticker object and the function `history` extract stock information and save it in a dataframe named `gme_data`.

![Alt text](./assets/screenshots/image12.png)

**Reset the index** using the `reset_index(inplace=True)` function on the gme_data DataFrame and display the first five rows of the `gme_data` dataframe using the `head` function.

![Alt text](./assets/screenshots/image13.png)

    2. Extracting Gamestop Revenue data

Use the `requests` library to download the webpage https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html. Save the text of the response as a variable named `html_data`.

![Alt text](./assets/screenshots/image18.png)

Parse the html data using `beautiful_soup`.

![Alt text](./assets/screenshots/image14.png)

Using `BeautifulSoup` or the `read_html` function extract the table with `GameStop Revenue` and store it into a dataframe named `gme_revenue`. The dataframe should have columns `Date` and `Revenue`.

![Alt text](./assets/screenshots/image15.png)

Display the last five rows of the `gme_revenue` dataframe using the `tail` function.

![Alt text](./assets/screenshots/image16.png)

    3. Gamestop dashboard

![Alt text](./assets/screenshots/image19.png)

# Licence

MIT