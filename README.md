# Excel_Airbnb
In this project, I'm doing data cleaning, data processing, data analysing, and data visualization on Microsoft Excel using real life data from (listed Airbnb on Naples, Italy)[]. This dataset containt 10999 entries
## Data Cleaning 
The steps for data cleaning:
1.	Fit row and column height as content.
2.	Set as table (ctrl + T).
3.	Delete blank column "neighbourhood_group".
4.	Freeze header row.
5.	Find duplicate row by "id" because id is unique value (there is not any duplicate row)
6.	Count entries/row by "=COUNT(A:A)".
7.	Find blank/null cell by "=COUNTBLANK(B2:B10999)", applied to every column.
8.	Found there are blank cell at columns "price", "last_review", "reviews_per_month", and "license".
9.	The blank cell at "price" column are going to filled with average price between the same "neighbourhood" (using pivot table).

10.	The blank cell at "last_review" and "reviews_per_month" column are left empty purposely, not 0.
11.	The blank cell at "license" column are filled with "Not provided".
12.	Set column type as it supposed to be (number, currency, text, date, etc).

## Data Processing

## Data Analysis 
## Data Visualization
## Insight
