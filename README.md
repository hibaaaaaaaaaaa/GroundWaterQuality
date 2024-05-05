
# Groundwater Quality Analysis Project

Groundwater is a natural resource for drinking water and requires regular assessment to ensure its quality. This study focuses on evaluating groundwater quality, specifically from wells, in a region of Northern Morocco. Water quality indices **(IQEs or WQI)** are used to assess the quality of groundwater, considering various physico-chemical and bacteriological parameters. This study compares three different **IQEs** to evaluate groundwater quality based on data collected from nine wells in the study area during **2016** and **2017**. The data collected is stored in the Excel file named `WaterQuality.xlsx`.


## Water Quality Indices Used
1. Weighted Arithmetic Mean Water Quality Index **(WAWQI)**
2. Weighted Geometric Mean Water Quality Index **(WGWQI)**
3. Oregon Water Quality Index **(OWQI)**

## Equations for Calculating IQEs
1. The Weighted Arithmetic Mean Water Quality Index (WAWQI) is calculated using the following equation:

&emsp; **WAWQI** = ∑(𝑖=1 to 𝑛) 𝑄𝑖 × 𝑊𝑖\
&emsp; Where :
- 𝑄𝑖 is the value of quality parameter i.
- 𝑊𝑖 is the weight assigned to parameter i, calculated as 𝑊𝑖 = 𝑤𝑖 / ∑𝑤𝑖 ,  𝑤𝑖 is provided in the Excel file `Paramètres1.xlsx`.



2. Weighted Geometric Mean Water Quality Index (WGWQI) is calculated using the following equation:

&emsp; **WGWQI** = ∏(𝑖=1 to 𝑛) (𝑄𝑖^𝑊𝑖) \
&emsp; Where :
- 𝑄𝑖 is the value of quality parameter i.
- 𝑊𝑖 is the weight assigned to parameter i, calculated as 𝑊𝑖 = 𝑤𝑖 / ∑𝑤𝑖 ,  𝑤𝑖 is provided in the Excel file `Paramètres1.xlsx`.

3. Oregon Water Quality Index (OWQI) s calculated using the following equation:

&emsp; **OWQI** = √(𝑛 / (∑(𝑖=1 to 𝑛) 𝑆𝐼_𝑖^2))\
&emsp; Where :
- 𝑛 is the total number of parameters, and 𝑆𝐼_𝑖 is the Subindex for parameter 𝑖 , provided in the Excel file.






 
## Quality Rating Equations
For each parameter 
𝑄𝑖, the quality rating is calculated using specific equations:
\
𝑄𝑖 = (𝐶𝑝𝐻 - 8.5)/(6.5-8.5)\
Where 𝐶𝑝𝐻 is the 𝑝𝐻 concentration.\
The quality rating for each parameter is then used in the calculation of **IQEs** to determine overall water quality indices.
​
 
​
​
 
## Interpretation of Results
1. **WAWQI Interpretation :**


| WAWQI Range             | Water Quality Level                                                               |
| ----------------- | ------------------------------------------------------------------ |
| WAWQI < 50 |Excellent Water    |
| 50 ≤ WAWQI ≤ 100 | Good Water   |
| 101 ≤ WAWQI ≤ 200  |  Poor Water   |
| 201 ≤ WAWQI ≤ 30 | Very Poor Water |
|WAWQI > 300| Unsuitable for drinking |

2. **WGWQI Interpretation :**



| WGWQI Range             | Water Quality Level                                                               |
| ----------------- | ------------------------------------------------------------------ |
| 90 ≤ WGWQI ≤ 100 |Excellent     |
| 70 ≤ WGWQI ≤ 89 | Good   |
| 50 ≤ WGWQI ≤ 69  |  Medium   |
| 25 ≤ WGWQI ≤ 49 | Bad |
|0 ≤ WGWQI ≤ 24| Very Bad |

3. **OWQI Interpretation :**


   
| OWQI Range             | Water Quality Level                                                               |
| ----------------- | ------------------------------------------------------------------ |
| 90 ≤ OWQI ≤ 100 |Excellent     |
| 85 ≤ OWQI ≤ 89 | Good   |
| 80 ≤ OWQI ≤ 84  |  Fair   |
| 60 ≤ OWQI ≤ 79 | Poor |
|0 ≤ OWQI ≤ 59| Very Poor |

## Code Implementation
The code implementation for calculating **WAWQI**, **WGWQI**, and **OWQI** from scratch and analyzing water quality data is provided in the `code.ipynb` file. The code includes the equations mentioned above along with functions to interpret the results and a pandas DataFrame for comprehensive analysis.

## Data Source
The data collected for this groundwater quality evaluation project is stored in the Excel file named `WaterQuality.xlsx`. The file `Parametres1.xlsx` contains the weights 𝑤𝑖 (with lowercase "w") and the subindices 𝑆𝑖 for each parameter, which are used in the calculations of the water quality indices.
## Authors

- [@Hiba SOFYAN](https://github.com/hibaaaaaaaaaaa)

