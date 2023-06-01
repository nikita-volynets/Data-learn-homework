# Module 3 - Homework

## 1. Create Superstore Dashboard in Tableau

My Superstore Dashboard is available on Tableau Public: https://public.tableau.com/app/profile/nikita.volynets/viz/MySuperstore_Dashboard_16855895573830/KPIDynamicDashboard



## 2. Create Survey for Anatytics reports business users


## 3. Create Airbnb Analytical Tool in Tableau

### 3.1 Cleansing data in Tableau Prep Builder

#### 3.1.1 Listing_summary

* Delete host_id, host_name - useless for our analysis, neighbourhood_group - null values
* Rename id -> lising_id, name -> listing_name

#### 3.1.2 Listing

* Leave only useful fields with additional details about listings that we would like to use in our analysis: 
**id, listing_url, picture_url, accomodates, bathrooms, bedrooms, beds, square_feet, price, weekly_price, monthly_price**
* Fields **square_feet, weekly_price and monthly_price** are not included due to big amount of null values (> 90%), it's not enough for analysis

#### 3.1.3 Calendar, Reviews_summary, neighbourhoods.geojson

* No changes

#### 3.1.4 Reviews, neighbourhoods

* Not included in the analysis
