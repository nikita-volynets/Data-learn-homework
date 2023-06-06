# Module 3 - Homework

## 1. Create Superstore Dashboard in Tableau

My Superstore Dashboard is available on Tableau Public: [My Superstore Dashboard](https://public.tableau.com/app/profile/nikita.volynets/viz/MySuperstore_Dashboard_16855895573830/KPIDynamicDashboard)

In my Dashboard I practiced and included the following Tableau features:

- Tableau Data Sources
- Live/Extract
- Dimensions/Measures/Filters
- Calculation Fields
- Parameters
- Table Calculations
- LOD
- Blending
- Federated Data Source
- Dashboard/View/Story
- Forecast/Trend/Clustering

## 2. Create Survey for Anatytics reports business users


## 3. Create Airbnb Analytical Tool in Tableau

### 3.1 Business Task

**About the company:** Real estate company - long-term rental with subsequent leasing the same property for a short period.

**Task:** Create an analytical tool that will allow to analyze the short-term rental housing market in London.

**Goal:** to choose the most attractive district and type of housing for investment

### 3.2 Dashboard Design

Using Canvas template collected all needed information about the Dashboard

![Canvas](https://github.com/nikita-volynets/Data-learn-homework/blob/bba638e65739138681c2d9f2cb455a50d339398c/Module%203/Images/Dashboard%20Canvas.jpg)

Based on the previous information created Dashboard Mock Up



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
