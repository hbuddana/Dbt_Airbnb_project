# Airbnb_dbt_project

# Airbnb Data Modeling and Transformation Project

## Overview

This project is dedicated to creating a robust data pipeline that takes raw Airbnb data and converts it into a structured, analytical model suitable for business intelligence tasks. This multi-layered approach ensures data integrity and usability for informed decision-making. Here's an overview of the project:

![1](https://github.com/hbuddana/Dbt_Airbnb_project/assets/65592890/d47bf69b-c42a-49e0-8ec2-d6bce48e09d6)



![3](https://github.com/hbuddana/Dbt_Airbnb_project/assets/65592890/f271fa06-ab46-4a24-b94c-70a93f7fd3be)



### Layers of Transformation

**Raw Layer**: The foundation of the pipeline, consisting of raw data tables:

- `raw_listings`: Raw data regarding Airbnb listings.
- `raw_hosts`: Raw data concerning Airbnb hosts.
- `raw_reviews`: Raw data of reviews left by guests.

**Staging Layer**: An intermediate layer where basic quality checks are applied:

- `src_listings`: Listings data undergoing initial checks.
- `src_hosts`: Hosts data subjected to basic validation.
- `src_reviews`: Reviews data going through preliminary checks.

**Core Layer**: The heart of the pipeline where data is cleaned and consolidated:

- `Hosts`: Data about hosts after cleansing operations.
- `Listings`: Enhanced listings data post-cleaning.
- `Reviews`: Refined reviews data ready for analysis.

**Presentation Layer**: The final layer optimized for consumption by analytical tools:

- `Listings mart table`: Aggregated data model for listings.
- `Reviews mart table`: Consolidated data model for reviews.

### Data Models

- **Listings**: Contains detailed information about Airbnb listings, including location, price, and host details.
- **Reviews**: Comprises reviews data linked to listings, complete with sentiment analysis.
- **Hosts**: Host information including identification, name, and status as a superhost.

![2](https://github.com/hbuddana/Dbt_Airbnb_project/assets/65592890/dcd4c7ad-8d5b-486b-aded-06ed5b8b88f8)

### Analytics and Business Intelligence

The processed data feeds into an executive dashboard, providing actionable insights into:

- Performance of listings.
- Satisfaction ratings from reviews.
- Host activity.

This empowers stakeholders to make data-driven decisions and strategic plans.

## Project Structure

The DBT (Data Build Tool) project is structured to support:

- Incremental builds.
- Full refreshes.
- Complex transformations.

It makes use of Jinja templating for dynamic SQL generation. This project is designed for scalability and maintainability to accommodate Airbnb's growing data while remaining robust and adaptable.


## Usage

Once the data models are in place, you can run various analyses to extract insights, such as:

- Analyzing host performance and identifying top-performing hosts.
- Examining listings data to understand pricing strategies and occupancy rates.
- Conducting sentiment analysis on reviews to gauge customer satisfaction and identify areas for improvement.

This project is a testament to the power of data transformation in extracting meaningful insights from raw data and presenting it in an accessible form for stakeholders to make informed, data-driven decisions.
