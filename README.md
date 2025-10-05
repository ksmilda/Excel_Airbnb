# Excel_Airbnb
In this project, I'm doing data cleaning, data processing, data analysing, and data visualization on Microsoft Excel using real life data from [listed Airbnb on Naples, Italy](https://insideairbnb.com/). This dataset containt 10699 entries and several columns. Take a look at dataset [here][].


## Data Cleaning 
The steps for data cleaning:
1. Fit row and column height;
2. Set as table (ctrl + T);
3. Delete blank column "neighbourhood_group";
4. Freeze header row;
5. Find duplicate row by "id" because id is unique column (there is not any duplicate row);
6. Count entries/row by "=COUNT(A:A)";
7. Find blank/null cell by "=COUNTBLANK(B:B)" (applied to every columns);
8. Found there are blank cell at columns "price", "last\_review", "reviews\_per\_month", and "license";
9. The blank cell at "last\_review" column are left empty purposely, not fill it with 0 or fake date because it will mess up the timeline;
10. The blank cell at "price" and "license" column are filled with "Not Provided";
11. The blank cell at "reviews\_per\_month" column are filled with "0";
12. Set column type as it supposed to (number, currency, text, date, etc).



## Data Processing
1. Add a new column "price_grouping" based on values on column "price" using "=IFS(I12="","Not Provided",I12<=200,"Low",I12<=1000,"Mid",I12<=5000,"High",I12>5000,"Luxury")";
2. Add new column "minimum_nights_grouping" based on "minimum_nights";
3. Add new column "host_status" based on last review, if there are not any reviews for the least 1 year then it is assumed as a non-active service;
4. Add new column "has_license" for licensed checking based on column "licensed". If licensed is not provided, then it shown as "Not Licensed";


## Data Analysis 
## Data Visualization


## Insight
