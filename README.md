# Netflix Analysis Dashboard (Power BI)

## Project Overview
This project presents an interactive Power BI dashboard designed to provide comprehensive insights into Netflix's TV show and movie content. A key highlight of this project is that the entire dashboard, including all metrics and interactive features, was developed **solely using Power Query for data transformation and Power BI's built-in visualization capabilities, without writing any DAX.**

This demonstrates the significant power and flexibility of Power Query for data preparation and how effective data storytelling can be achieved through meticulous data modeling and intuitive visual design.

## Tools used
*  **Power BI:** For data visulidsation.
*  **Power Query:** For data transformation.
*  **Excel:** For Data cleaning.
*  **Kaggle:** For Dataset.

## Dataset
The dashboard is built upon a dataset of Netflix TV shows and movies, comprising 12 key columns:
`show_id`, `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`.

**Dataset:** https://lnkd.in/dYTi-STA

## Dashboard Features & Key Insights
* **Key Performance Indicators (KPIs):**
    * **Total Shows:** Overall count of all content.
    * **Movie & TV Show Count:** A clear breakdown of content by type.
    * **Total Directors:** Count of unique directors.

* **Content Trends & Distribution:**
    * **Yearly Release:** Visualizes the trend of content added over time, showing peaks and valleys in production/addition.
    * **Shows Released by Countries:** Highlights the top countries producing content for Netflix, indicating key strategic regions.
 
* **Content Breakdown & Audience Insights:**
    * **Genres:** Identifies the most prevalent genres within the Netflix library. This was achieved by splitting and unpivoting the multi-value `listed_in` column in Power Query.
    * **Maturity Ratings:** Shows the distribution of content based on audience ratings (e.g., TV-MA, TV-14, PG), offering insights into target demographics.

* **Interactive Filtering & Exploration:**
    * **Type Slicer:** Buttons (`Movie` / `TV Show`) allow users to quickly filter the entire dashboard to focus on a specific content type.
    * **Range of Year Slicer:** Enables filtering content by its release year.
    * **List of Shows:** A slicer to select individual titles, which then displays their respective `Description`.

## Technical Approach (No DAX!)
The entire data preparation and transformation process was meticulously handled within **Power Query Editor**:

* **Data Loading:** Directly importing the Netflix dataset.
* **Data Cleaning & Type Conversion:** Ensuring correct data types for each column.
* **Splitting & Unpivoting:** The `listed_in` column, which contains comma-separated genres, was split by delimiter and then unpivoted to create individual genre entries for accurate counting and analysis.
* **Basic Aggregations:** Core metrics and counts (like Total Shows, Movie/TV Show counts, genre counts) were derived using Power Query's grouping and aggregation functionalities.

This approach demonstrates proficiency in robust ETL (Extract, Transform, Load) processes within Power BI's native environment.


## Future Enhancements (Potential DAX Applications)

While this dashboard successfully avoids DAX, future enhancements could include:

* **Time Intelligence:** Calculating Year-over-Year growth rates for content addition using DAX.
* **Advanced Ratios:** Creating measures for percentage of total content by specific directors or genres.
* **User-Defined Metrics:** Allowing users to dynamically switch between different aggregation types.

## Screenshot
* **Dashboard Preview:** 
![dashboard](https://github.com/ramss8/NETFLIX-Analytics/blob/main/Netflix%20Dashbord%20Snapshot.jpg)
* **Dashboard Video Demonstration:** https://github.com/ramss8/NETFLIX-Analytics/blob/main/Netflix%20Dashboard%20Video%20Demonsration.mp4

## Author
[Ram Sharma]
