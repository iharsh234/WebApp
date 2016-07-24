# WebApp
Assignment:
Anand recently read a scientific paper where he learned about momentum
investing. He learnt that stocks that go up in recent past would continue to go up in
recent future. He learnt that a portfolio with such stocks does better than market on
average. He is excited with the idea and wants to test this hypothesis/finding
himself.

Anand logs on to xyz.com to do his analysis. Smart engineers at Xyz
want to help Anand to find the truth about financial markets in an analytical way.
Now, Anand wants to do the following:
1. Select stocks that have gone up in recent past

2. Check whether those stocks have gone up in future too.

You are asked to help Anand achieve this task through this web application.
Now you need to create a web application that allows Anand to

1. Specify a list of stock symbols on a form. Examples of stock symbols are
TATAMOTORS;ICICIBANK;VOLTAS;
Find the list of stocks here:
https://www.nseindia.com/content/indices/ind_niftynext50list.csv

2. Specify a date range with a start date and an end date. The start date should
be later than 2016-01-01 and end date should later be than start date and not
later than today’s date.

3. Provide an option to start the analysis by calling the API mentioned below
with the parameters specified above.

4. To perform the analysis the web application should

a. Make a query to external API (Quandl) to fetch data for stocks listed in
text box in (1) between start and end dates. Below is the format for
the API call:
https://www.quandl.com/api/v3/datasets/NSE/SYMBOL.json?api_ke
y=gWf2CLShwrGUBVnqzsT4&start_date=yyyy-mmdd&
end_date=yyyy-mm-dd

b. Learn about the output response by running the sample query in a
browser:
https://www.quandl.com/api/v3/datasets/NSE/TATACHEM.json?api_key=g
Wf2CLShwrGUBVnqzsT4&start_date=2015-07-05&end_date=2016-05-05

c. On retrieving the data, divide the date into two equal parts. Let’s call
two parts as past data (part 1) and future data (part 2). Calculate two
values Rpast and Rfuture where

i. Rpast = log (last value of part 1/first value of part 1)

ii. Rfuture = log (last value of part 2/first value of part 2)

5. Display the result of the analysis as

a. Display in a table Symbol/ Rpast / Rfuture.

b. Display the top 10% stocks by Rpast (Table Columns: Symbol/ Rpast
/Rfuture) in the display

c. Display the bottom 10% stocks by Rpast (Table Columns: Symbol/ Rpast
/Rfuture)

d. Display Averages of Rfuture from tables in 5b (Positive Momentum) and
5c (Negative Momentum). This table will have one row with three
columns (Positive Momentum, Negative Momentum, Positive
Momentum – Negative Momentum)

6. Looking at the table in 5d, Anand will make a crude judgement about
momentum trading performance.


Additional tasks after completing the above
7. Make the table in 5a sortable.
8. Plot histogram of table in 5b and 5c.
9. Add calendar feature to date-picker in the user form.
10. Add a feature of your choice
11. Add a feature of your choice

##########################  TODO ######################

1. Intergrate AJAX calls to external API.

2. 4(c) to 11

