Project Overview

This project aims to select the most suitable wind turbine model for a potential wind energy project using data collected from a wind mast (meteorological mast). The wind mast data includes wind speed, wind direction, and other meteorological parameters collected over a specified period. By analyzing this data, we can assess the wind resource at the site and determine which wind turbine model would provide the best performance.

Data Sources

	1.	Wind Mast Data:
	•	Wind Speed: Measured at multiple heights (e.g., 125m, 100m, 93m, 75m and 50m) using anemometers.
	•	Wind Direction: Measured using wind vanes.
	•	Turbulence Intensity (TI): Information on the variability of wind, crucial for determining the structural demands on turbines.
	2.	Turbine Specifications:
	•	Manufacturer data sheets providing key specifications for different wind turbine models, including:
	•	Cut-in wind speed (minimum wind speed for turbine operation).
	•	Rated wind speed (optimal speed for maximum power output).
	•	Cut-out wind speed (maximum safe wind speed before turbine shuts down).
	•	Power curve: A graph showing the turbine’s power output at different wind speeds.

Tools and Technologies

	•	Python for data analysis and visualization.
	•	Pandas/NumPy for handling wind mast data.
	•	Matplotlib/Seaborn for visualizing wind speed distributions and power curves.
	•	Excel/CSV files for the wind mast dataset and turbine specifications.

Steps for Analysis

1. Data Preprocessing

	•	Load Data: Import the wind mast data (CSV) into your data analysis tool.
	•	Clean Data: Remove any missing or erroneous values.
	•	Wind Speed Aggregation: If the data was collected at multiple heights, aggregate or interpolate the wind speed values to match the hub height of the potential wind turbine (e.g., 125m).

2. Wind Speed Analysis

	•	Descriptive Statistics: Compute mean, median, and standard deviation of wind speed at the site.
	•	Wind Speed Distribution: Plot the wind speed frequency distribution (histogram) to visualize the wind resource. This will help identify the most common wind speeds at the site.

6. Final Recommendation

	•	Based on the wind resource assessment and turbine power curve, energy yield estimation is done to find the suitable turbine for the site.
	•	Annual Energy Production: Computed energy estimation for 3 turbine models.

Visualization and Reporting

	•	Wind Speed Distribution: Visualize the site’s wind speed distribution using histograms.
	•	Power Curves: Plot the power curves of the selected turbines against the site’s wind speed distribution to compare expected performance.
	•	Turbulence Intensity: Display turbulence intensity to highlight the site’s wind variability.
	

Conclusion

After completing the analysis, the most suitable turbine model should be selected based on:

	•	Energy Production: Highest annual energy yield (AEP) based on the site’s wind conditions.


File Structure

|   |-- Mast1_zone42_wgs84_473066_2600838.csv        # Raw wind mast data (wind speed, direction, temperature, etc.)
|   |-- Power_curve.csv          # Turbine models with power curves and specifications
|
|-- notebooks/
|   |-- EDA_Project_Group-2.ipynb   # Code for cleaning and preparing the data
|  
|-- results/
|   |--EDA_Project_Group-2.pptx
|
|-- readme.EDA_Project_Group-2.md                   
 # Project overview and instructions
Dependencies

	•	Python 3.x
	•	Pandas, NumPy, Matplotlib, Seaborn (Python)
	•	CSV data files (for wind mast and turbine data)

How to Run the Project

	1.	Clone the repository.
	2.	Install necessary Python libraries:
		pip install pandas numpy matplotlib seaborn windrose
	3.	Place wind mast data and turbine specifications in the data/ 		directory.
	4.	Run the Jupyter notebooks in sequence to perform the 		analysis and obtain the results.

This README file provides a structured guide for performing wind mast data analysis and selecting the most suitable turbine.