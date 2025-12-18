PROJECT OVERVIEW

This project analyzes the distribution of metered parking spaces across different districts and regions in Hong Kong using Power BI. The dashboard highlights key metrics, vehicle type breakdowns, and geographic patterns to support insights into urban planning and transport management.

DATASET

Source: data.gov.hk 

Dataset: Distribution of Metered Parking Spaces at Different Districts in Hong Kong.

Fields Used: Region/ District/ Location / Types of Operating Hours/ Parking spaces for Private Cars, Goods Vehicles and Coaches

PROCESS
1. Data Import
   - Imported raw dataset into Power BI.
   - Renamed columns for clarity. (PrivateCarSpaces, GoodsVehicleSpaces, CoachSpaces).
2. Data Cleaning
   - Trimmed and standardized text fields (Region, District, Location)
   - Created a lookup table for Operating Hours codes with full descriptions.
3. Data Modeling
   - Built a star schema
   - Established relationships between tables. (Raw data and operating hour description)
4. DAX Measures
   - Total Spaces = SUM('Region (dataset)'[Private Cars Spaces]) +SUM('Region (dataset)'[Goods Vehicle Spaces]) +SUM('Region (dataset)'[Coach Spaces])
   - Private Car Spaces = SUM('Region (dataset)'[Private Cars Spaces])
   - Goods Vehicles Spaces = SUM('Region (dataset)'[Goods Vehicle Spaces])
   - Coachs Spaces = SUM('Region (dataset)'[Coach Spaces])
5. Visualization
   - Cards: Total spaces, breakdown by type.
   - Map: Geographic distribution of parking spaces by region.
   - Bar Chart: District comparison by vehicle type.
   - Donut Chart: Proportional breakdown of vehicle types.
   - Slicers: Region

**i. Create relationship**
<img width="1466" height="784" alt="image" src="https://github.com/user-attachments/assets/2eaa6479-ad89-4450-8aa0-76e166d69ed0" />

**ii. Dashboard for Overview**
<img width="1415" height="798" alt="image" src="https://github.com/user-attachments/assets/83f814fe-1380-449c-8350-bbc467f1f2a8" />

**iii. Dashboard for Operating Hours**
<img width="1408" height="798" alt="image" src="https://github.com/user-attachments/assets/46f6dad7-9837-4716-aa14-3bc32da9cd41" />

**iV. Dashboard for Location Detail**
<img width="1411" height="798" alt="image" src="https://github.com/user-attachments/assets/211ebef7-93b6-463e-9bb4-3c7d53a8e673" />



       



