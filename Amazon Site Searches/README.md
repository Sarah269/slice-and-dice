## DATABASE: ONSITE_SEARCH_PRODUCT_DEMAND_ANALYSIS_ON_RETAIL_SITES_AND_MARKETPLACES
- Snowflake marketplace database
- SCHEMA:  DATAFEEDS
- TABLE: ON_SITE_SEARCH
- Database of search terms used on Amazon.com from 1/1/21 to 6/20/22
- Search terms are in free form
- Number of Users, Number of visits
- 7 million rows

# Tasks performed:
- Ranked search terms for each date based on the sum of calibrated users.
- Selected top 10 search terms for each date. 5702 rows.
- Select distinct search terms for the above results, 294 rows.  Exported to a csv file.
- Imported csv file to Google Sheets.  Added a new column, keyword_category.
- Categorized the search terms with the assistance of Amazon.com.
- Exported annotated Google Sheets file to csv.  Created a table in Snowflake and loaded csv file.
- Joined newly created table to On_site_search table resulting in a table with the columns of on_site_search and the new column keyword_category.
- Extracted the results to a csv file.  5702 rows.
