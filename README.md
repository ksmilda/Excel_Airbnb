# Excel_Airbnb

In this project, I'm doing data cleaning, data processing, data analysing, and data visualization on Microsoft Excel using real life data from [Airbnb listings on Naples, Italy](https://insideairbnb.com/) to explore patterns in pricing, availability, and host licensing status. The goal was to design an interactive Excel dashboard using PivotTables, charts, and slicers to uncover insights about Airbnb market behavior. This dataset containt 10699 entries and several columns. Take a look at dataset [here](/airbnb_naples1.xlsx).


<img width="1913" height="584" alt="image" src="https://github.com/user-attachments/assets/becf97c3-a3e4-4731-b574-f4a557b768c9" />


## Data Cleaning (Preparation)
The steps for data cleaning:
* Verified and standardized data types for key numeric and date columns (price, minimum_nights, last_review, etc.);
* Find duplicate entries (by "id") and removed it (there is not any duplicate entries);
* Left blank cells in "last_review" (type column: date) to accurately represent listings with no reviews (indicating no guest feedback yet);
* The blank cell at "price" and "license" column are filled with "Not Provided";
* The blank cell at "reviews_per_month" column are filled with "0";


<img width="1919" height="533" alt="image" src="https://github.com/user-attachments/assets/00af1755-46dd-4faa-bf04-29beee97d9d4" />


## Data Processing
* Created calculated column "price_grouping" based on values on column "price" (group prices into "Not Provided","Low","Mid","High","Luxury");
* Created calculated column "minimum_nights_grouping" based on "minimum_nights";
* Created calculated column "host_status" based on last review, if there are not any reviews for the last 12 months then it is assumed as a non-active listings;
* Created calculated column "has_license" for licensed checking based on column "licensed". If licensed is not provided, then it shown as "Not Licensed" or "Exempt";


## Data Analysis 
* Built multiple PivotTables to summarize listings by:
  + Room type, Neighbourhood, License Status, and Price Category.
  + Average Price and Total Listings per Neighbourhood
  + Minimum Nights vs Price relationship
* Added slicers to make the dashboard interactive — users can filter by price category, neighborhood, room type, or license status.
* Used bar, column, and donut charts for visual clarity and comparison.

## Data Visualization
Take a look at the interactive dashboard [here](https://1drv.ms/x/c/b693fc09892146b6/ERyKY92nSQRJkEm7F_nhtX4Bvol8jBQzaPP9YAZHxAeD_A?e=PplMbu&nav=MTVfe0RFNzc3NENCLUEwMzEtNEMyOS1CMEM0LTk3NzkxMDFBRDcyM30).


This dashboard highlights a market characterized by budget-friendly listings, strong licensing compliance, and a dominance of private accommodations.
Neighborhoods like Chiaiano and San Giuseppe stand out for their premium pricing, while San Lorenzo and San Ferdinando lead in total listing volume — key insights for investors or policy planners analyzing Airbnb activity distribution.

<img width="1115" height="611" alt="image" src="https://github.com/user-attachments/assets/9a7c78d2-95a6-44f7-8d93-62c1294d9aac" />



## Insight
* Listings without a license make up a significant portion of the dataset, indicating possible compliance issues in some areas.
* Higher prices are concentrated in specific neighborhoods, showing localized demand and premium zones.
* Most listings have short minimum night requirements, which aligns with short-term visitor patterns.
* The correlation between minimum nights and price suggests that hosts offering longer stays often set higher prices.

* Based on neighbourhodd, Chiaiano and San Giuseppe have the highest average prices meanwhile San Lorenzo and San Ferdinando have the most listings overall.
* Based on price, most listings fall in the Low price range indicating Airbnb is mainly budget-friendly. Even there are Luxury and High categories which are very limited.
* Entire homes/apartments (63%) and private rooms (36%) dominate the market, but few shared or hotel rooms are available.
* Majority of listings are licensed, but a small portion are unlicensed/exempt.
* Long-term stays (30+ nights) have the highest average price. 1-night stays are also relatively higher, likely for short visits or weekends.


## What I Learned
* Hands-on experience with Excel dashboarding techniques — PivotTables, slicers, and chart interactivity.
* Better understanding of data cleaning logic, especially how missing values can represent real conditions (e.g., no reviews).
* Improved ability to derive data-driven insights from visual storytelling and summary tables.
* Practice in structuring and presenting an analytical project for a professional audience.
