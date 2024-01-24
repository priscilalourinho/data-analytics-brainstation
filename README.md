[![author](https://img.shields.io/badge/author-priscilalourinho-blue.svg)](https://www.linkedin.com/in/priscilalourinho/)

# Data Analytics Final Project - Brainstation

# **Initializing Data Exploration: Library Import and DataFrame Loading**

#### The dataset includes information on causes of death and the corresponding mortality rate per 100,000 inhabitants from 2018 to 2022. Tables were tailored based on the features provided on the Statistics Canada website. You can access the customized table here:

[Deaths and mortality rate (age standardization using 2011 population), by selected grouped causes](https://www150.statcan.gc.ca/t1/tbl1/en/cv!recreate.action?pid=1310080001&selectedNodeIds=1D2,1D11,4D1,4D2&checkedLevels=0D1,1D2,2D2&refPeriods=20180101,20220101&dimensionLayouts=layout3,layout3,layout3,layout3,layout2&vectorDisplay=false)

#### To keep things simple and considering the time available for the analysis project, We focused on the province of British Columbia (BC).

#### For comparison purposes, we decided to include data for the entire country, Canada, as well as a province with lower population density than BC; in this case, we chose Newfoundland and Labrador.

# **Exploring Patterns in Causes of Death through Fundamental Statistical Analysis**

 The three blocks of code below follows a consistent pattern, generating statistics like **mean, median, standard deviation, minimum, and maximum** for Canada (CA), British Columbia (BC), and Newfoundland and Labrador (NL).

All of them include the same types of plots: **normal curve, box plot, scatter plot, histograms, bar plots, and Pareto charts.**

The goal is to **use visual representations to better understand how causes of death behave based on the sample data we have**.


## **Quick guide to understand the plots:**

→ **Normal Curve:**
It's a curve that shows how data is spread out. **Most data points are in the middle, and fewer are on the sides.**

→ **Box Plot:**
It's a box-shaped that provides a visual summary of the distribution of a dataset. ***It shows the median, quartiles, and potential outliers.***

→ **Histogram:**
A histogram is a bar chart that displays the distribution of a continuous dataset. It divides the data into intervals (bins) and represents the frequency of values within each bin. ***It provides insights into the shape and central tendencies of the data.***

→ **Pareto Chart:**
A Pareto chart combines both bar and line graphs. It arranges categories in descending order by frequency or impact. The left vertical axis represents the frequency or count, while the right vertical axis represents the cumulative percentage. ***It helps identify the most significant factors in a dataset.***

# **Statistical Conslusions, Defining Next Steps, and Exporting Results**

### **Normal Curve (bell curve)**
##### The lack of symmetry in the normal curves, with the peak shifted to the right, suggests a concentration of values at zero (indicating causes of death with a low occurrence in the population), another cluster in the low-to-moderate range, and a few extreme values on the right (indicating causes of death with a high occurrence in the population).

##### The lack of symmetry, while not immediately noticeable in the curve, becomes apparent when confirming that the peak of the bell does not align with zero on the x-axis.

### **Box Plot**

Across all three analyses, the proximity of the median to the minimum value indicates a positive skewness in the data. In a positively skewed distribution, the majority of data points cluster towards the lower end, with fewer extreme high values. In the context of this analysis, these extreme high values represent the more prevalent causes of death within the population.

### **Histogram and Pareto chart**

In both charts, we can infer that a small number of death causes have a significant impact on the overall causes of death regardless of the size of the province or country wise.

The bars more to the left indicates the causes of death that dominate each one of the distribuitions(high-frequency or high-impact factors).


### **Final Conclusion**
The visual analysis of the plots suggests that a limited number of categories or values exert a substantial impact, while the majority exhibit lower impact or occurrence.

It's crucial to note that employing an outlier removal approach, such as ZScore, could notably influence statistical measures like the mean and standard deviation. Such measures may deviate from representing the true characteristics of the distribution due to the inherent skewed nature of the data.

Recognizing that the skewed distribution may contain valid and meaningful observations, we opt to proceed with the analysis, focusing on the top 10 causes of death. This approach allows us to delve into the most influential factors while retaining a comprehensive understanding of the data's underlying characteristics.
