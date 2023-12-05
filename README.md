# Nashville Housing Data Cleaning

![](header.png)

## Introduction
Data cleaning, also known as data cleansing, is the process of identifying and correcting or removing errors, inconsistencies, and inaccuracies in data. It is a critical step in the data analysis process that ensures that data is accurate, consistent, and usable for analysis.

The process of data cleaning can involve various tasks, such as:

1. Removing duplicate data: This involves identifying and removing any duplicated data entries in the dataset.

2. Handling missing data: This involves identifying missing data values and deciding on an appropriate strategy to handle them, such as imputing missing values or removing the entire observation.

3. Correcting inconsistencies: This involves identifying inconsistencies in data, such as data entry errors or data that does not conform to a specific format or standard.

4. Standardizing data: This involves converting data into a common format, unit of measure, or data type.

5. Removing outliers: This involves identifying data points that are significantly different from other data points and deciding on an appropriate strategy for dealing with them, such as removing them or transforming them.

6. Validating data: This involves checking the accuracy of data, such as ensuring that numerical data falls within a valid range.

Data cleaning is an iterative process and requires careful attention to detail to ensure that the resulting data is accurate and usable for analysis.

## About the dataset

The dataset contains Home value data for Nashville housing the capital city of U.S. state of Tennessee. The dataset contains 19 columns and 56,477 rows of data.

Click [here]() to download the dataset

## Metadata

- UniqueID : id number attributed to a buyer.
- ParcelID : code attributed to a property.
- LandUse : different uses of the land.
- PropertyAddress : address of the property
- SaleDate : date the property was sold
- SalesPrice : cost of the property
- LegalReference : citation is the practice of crediting and referring to authoritative documents and sources.
- SoldAsVacant : used to describe a situation in which property is vacant when it is sold so that the new owner can move in immediately
- OwnerName : name of property owner
- OwnerAddress : address of the owner
- Acreage : the size of an area of land in acres
- TaxDistrict : region or locality that assesses real estate taxes on the properties located within its borders
- LandValue : worth of the land
- BuildingValue : worth of a building
- TotalValue : landvalue + building value
- YearBuilt : year the building was built
- Bedrooms : number of bedrooms in the property
- FullBath : a bathroom that includes a shower, a bathtub, a sink, and a toilet.
- HalfBath : a half bathroom only contains a sink and a toilet.

Raw Data

![](raw_data.png)

## Tool

This project was carried out using Microsoft Sequel Server

## Data Cleaning

After downloading the dataset a database was created in sequel sever named **Nashville**, then imported the data using sequel sever import/export tool.

The following was discovered after exploring the dataset

- The SaleDate is not in the standard format.
- Some rows in the PropertyAddress column are NULL
- The PropertyAddress has both the City and House Address in the same column.
- The OwnerAddress has the state, city, and address in the same column.
- Some rows in the SoldAsVacant has Y and N instead of Yes or No.
- There are some duplicate rows that need to be removed.
- Some Columns would not be useful for the analysis and therefore should be deleted.
  
After cleaning the data, new columns were created in the table and updated with the cleaned data.


