# Subway Incident Analysis
## Samin Yasar Chowdhury
## Overview

This repository contains a Python notebook for analyzing subway incident data. The analysis focuses on understanding the patterns and trends of major subway incidents over time. The dataset used in this analysis is sourced from the MTA Subway Major Incidents dataset, which includes information about incidents from 2020 onwards.

## Dataset

The dataset used in this analysis is titled `MTA_Subway_Major_Incidents__Beginning_2020_20250207.csv`. It contains the following columns:

- `month`: The month in which the incident occurred.
- `division`: The division within the subway system where the incident occurred.
- `line`: The specific subway line affected by the incident.
- `day_type`: Indicates whether the incident occurred on a weekday or weekend.
- `category`: The category of the incident (e.g., Signals, Subway Car, Track, etc.).
- `count`: The number of incidents recorded.

## Analysis

The analysis is divided into several sections:

1. **Data Loading and Initial Exploration**: The dataset is loaded and the first few rows are displayed to get an initial understanding of the data.

2. **Data Cleaning**: 
   - Handling missing values in the `division` and `line` columns by filling them with 'Unlabeled'.
   - Converting the `day_type` column from binary values (1 and 2) to more descriptive labels ('weekday' and 'weekend').
   - Renaming columns for better readability.

3. **Monthly Incident Analysis**:
   - Extracting the month and year from the `date` column.
   - Grouping the data by month and summing the incident counts to analyze monthly trends.
   - Visualizing the monthly incident counts using a line plot.

4. **Visualization**:
   - A line plot is generated to show the trend of major incidents occurring each month over the years.

## Requirements

To run the notebook, you will need the following Python libraries:

- `pandas`
- `matplotlib`

You can install these libraries using pip:

```bash
pip install pandas matplotlib
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/saminyc/Subway_Data_Analysis.git
   ```

2. Navigate to the repository directory:

   ```bash
   cd Subway_Incidents_Analysis
   ```

3. Open the Jupyter notebook:

   ```bash
   jupyter notebook Subway_Incidents_Analysis.ipynb
   ```

4. Run the notebook cells to perform the analysis and generate visualizations.

## Results

The analysis reveals trends in subway incidents over time, highlighting months with higher incident counts. The visualizations provide insights into the distribution of incidents across different categories and days of the week. 

Some key insights found:

- **Peak Incident Year**: 2024 recorded the highest number of subway incidents (783), while 2020 had the lowest (322).
- **Monthly Trends**: December saw the most incidents (286), while April had the fewest (197).
- **Track Division Comparison**: More incidents occurred in B Division Tracks (1,469) compared to A Division Tracks (1,182).
- **Category Analysis**: The category "Persons on Trackbed/Police/Medical" had the highest number of incidents.
- **Unidentified Trains**: There are 4 trains with unlabeled or unidentified names.
- **Line-Specific Incidents**: Line 6 had the most incidents (218), while S Rock had the least (2) over the 4-year span.
- **Weekday vs. Weekend**: Incidents were more frequent on weekdays (2,372) than on weekends (283).
  
## Contributing

Contributions are welcome! If you have any suggestions or improvements, please open an issue or submit a pull request.

## Acknowledgments

- The dataset is provided by the Metropolitan Transportation Authority (MTA).
- Special thanks to the open-source community for providing the tools and libraries used in this analysis.

---

Feel free to explore the notebook and contribute to the analysis!
