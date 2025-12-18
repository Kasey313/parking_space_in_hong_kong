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




       



