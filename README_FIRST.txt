# PM07-PS01: The Five Steps of Data Analysis

## CityConnect Municipal Service Delivery Analysis

### 1. Project Overview

This project analyses a fictional municipal service-delivery dataset from CityConnect using Python, Pandas, NumPy and data visualisation libraries.

The main objective is to understand how long municipal service requests take to resolve and determine whether certain service types or geographical regions experience longer resolution times.

The findings will help CityConnect management identify operational challenges, prioritise resources and improve service-delivery efficiency.

### 2. Business Problem

CityConnect management wants to understand whether municipal service requests are being resolved within reasonable timeframes.

Long resolution times can negatively affect resident satisfaction, increase operational pressure and make resource planning more difficult.

This analysis investigates resolution times across different service types and regions to identify areas that may require operational improvements.

### 3. Dataset Description

The dataset contains 400 municipal service requests.
Each row represents one service request.

**Dataset variables include:**
- `opened_on`: Date and time the service request was opened.
- `status`: Current status of the service request.
- `service_type`: Category of the municipal service.
- `region`: Geographical region where the request originated.
- `resolution_days`: Number of days taken to resolve a request.
- `satisfaction_rating`: Resident satisfaction rating.

**Dataset coverage:**
- Total requests: 400
- Resolved requests: 360
- Open requests: 40
- Service types: 5
- Regions: 5
- Date range: 6 January 2026 – 23 June 2026

### 4. Why Open Requests Were Excluded

The analysis focuses on the 360 resolved service requests.

The 40 Open requests were excluded because they have not yet been completed and therefore do not have a final resolution time.

Including Open requests in the resolution-time calculations could produce misleading results because their actual completion times are not yet known.

### 5. The Five Steps of Data Analysis

#### PA0101: Describe the Size of the Sample

The dataset was examined to determine its size and structure.

Key findings:
- 400 total service requests.
- 360 resolved requests used for analysis.
- 40 open requests excluded.
- 5 service types.
- 5 geographical regions.

#### PA0102: Describe the Centre of the Data

Mean and median values were calculated to understand typical resolution times and resident satisfaction.

Key findings:
- Mean resolution time: 9.31 days.
- Median resolution time: 5.85 days.
- Mean satisfaction rating: 3.63.
- Median satisfaction rating: 4.0.

The median is recommended as the main measure of typical resolution time because it is less affected by unusually long delays.

#### PA0103: Describe the Spread of the Data

The range, interquartile range and standard deviation were calculated.

Key findings:
- Minimum resolution time: 0.4 days.
- Maximum resolution time: 73.1 days.
- Range: 72.7 days.
- Interquartile range (IQR): 8.52 days.
- Standard deviation: 10.34 days.

The IQR provides a more reliable indication of the spread of typical resolution times because it is less affected by extreme values.

#### PA0104: Assess the Shape of the Distribution

A histogram and boxplot were created to understand the distribution of resolution times.

Key findings:
- Skewness: 2.8.
- The distribution is strongly right-skewed.
- The mean is higher than the median.
- Some requests take significantly longer to resolve than most others.

The outliers may indicate operational challenges such as resource shortages, technical difficulties or delays in assigning technicians.

#### PA0105: Compare Data from Different Groups

Resolution times were compared across five service types and five geographical regions using count, mean, median and standard deviation.

**Service type comparison:**

| Service type | Mean days | Median days |
|---|---:|---:|
| Waste | 3.44 | 3.10 |
| Sanitation | 4.82 | 3.60 |
| Electricity | 7.56 | 5.85 |
| Roads | 11.21 | 8.30 |
| Water | 15.64 | 12.05 |

**Regional comparison:**

| Region | Mean days | Median days |
|---|---:|---:|
| CBD | 6.13 | 4.35 |
| North | 7.75 | 5.35 |
| East | 8.38 | 6.50 |
| West | 11.01 | 6.10 |
| South | 12.48 | 7.15 |

### 6. Main Findings

The analysis identified the following important findings:

1. Water services have the longest resolution times, with a mean of 15.64 days and median of 12.05 days.
2. Waste services have the shortest resolution times, with a mean of 3.44 days and median of 3.10 days.
3. The South region has the longest average resolution time at 12.48 days.
4. The CBD region has the shortest average resolution time at 6.13 days.
5. The overall resolution-time distribution is strongly right-skewed, suggesting that a smaller number of requests experience significant delays.

### 7. Recommendations to Management

Based on the findings, the following recommendations are proposed:

- Prioritise improvements in the Water service department.
- Investigate operational challenges affecting service delivery in the South region.
- Investigate unusually long resolution times to identify the underlying causes of delays.
- Review resource allocation, technician scheduling and departmental coordination.
- Monitor both mean and median resolution times regularly.
- Use the Waste department and CBD region as potential examples of more efficient service delivery.

These improvements could help reduce resolution times, improve resource utilisation and increase resident satisfaction.

### 8. Technologies Used

The following tools and libraries were used:

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- GitHub

### 9. Project Structure

The GitHub repository contains the following files:

```text
PM07-PS01-CityConnect-Analysis/
│
├── README.md
├── PM07-PS01.ipynb
├── cityconnect_service_requests.csv
│
└── outputs/
    ├── summary_file_1.csv
    ├── summary_file_2.csv
    └── summary_file_3.csv
```

The three output filenames above should be replaced with the actual filenames generated by the notebook.

### 10. How to Run the Notebook

1. Download or clone this public GitHub repository.
2. Extract the project folder if downloaded as a ZIP file.
3. Ensure that the notebook, original CSV and outputs folder remain in the same project directory.
4. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

5. Open a terminal in the project directory.
6. Launch Jupyter Notebook:

```bash
jupyter notebook
```

7. Open the project notebook.
8. Restart the kernel and run all cells from beginning to end.

The notebook performs the data analysis, generates visualisations and exports summary tables into the outputs folder.

### 11. Conclusion

This project demonstrates how the five steps of data analysis can be applied to a real-world business problem using Python.

The findings show that although most CityConnect service requests are resolved within a relatively short period, certain service types and geographical regions experience significantly longer delays.

Water services and the South region require particular management attention.

By using these findings to guide operational improvements and resource allocation, CityConnect can work towards more efficient service delivery and improved resident satisfaction.

---

Project: PM07-PS01 – The Five Steps of Data Analysis  
Learning Institution: Zaio Institute of Technology  
Learning Path: Data Science Bootcamp  
Author : Peter Mavazhe

