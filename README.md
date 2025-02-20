# Dataset of Currency Forward Position of U.S. International Fixed Income Funds

**Description**: We present an interactive dashboard visualizing the net position of each currency derivative of mutual funds which is used to manage their currency exposures. 
    Here we collect the dataset of currency forward contracts for major currencies used by U.S. international fixed-income funds.

**Created**: 2025-02-12  
**Updated**: 2025-02-20  

**Licenses**:  
- [Open Data Commons Public Domain Dedication and License v1.0](http://opendatacommons.org/licenses/pddl/)

**Sources**:  
- [EDGAR system](https://www.sec.gov/search-filings/mutual-funds-search)

## Measurement of fund currency forwards
For each fund `f`, currency `c`, and year-quarter `t`, we define the Net Forward Sales (NFS) at currency level as follows:
![image](https://github.com/user-attachments/assets/4e2d8a15-777c-4a43-b142-32fc9dedfbe5)
## Dashboard Features

- **Area Chart:** Shows the evolution of net forward sale positions over time for one or more selected currencies.
- **Horizontal Bar Chart:** Displays a broader picture of net forward sale positions per currency for a selected year end date.


## Visual Output
<iframe 
  src="https://LennoxFang.github.io/HedgingPlot/area_chart.html" 
  width="1200" 
  height="1200" 
  frameborder="0">
</iframe>
<iframe src="https://LennoxFang.github.io/HedgingPlot/bar_chart.html" width="100%" height="1200" frameborder="0"></iframe>

*Note:*  
- To view the interactive dashboard, you can run the provided Jupyter Notebook (`CurrencyForward_plot.ipynb`) locally.

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/LennoxFang/HedgingPlot.git
   cd HedgingPlot
