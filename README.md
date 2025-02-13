---
datapackage:
  title: Dataset of Currency Derivatives Position of U.S. international fixed income funds.
  description: We present an interactive dashboard visualizing the net Position of each currency derivative of mutual funds in order to manage their currency exposures. Here we collect the dataset of currency forward contracts used by U.S. international fixed income funds.
  created: 2025-02-12
  updated: 2025-02-13
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  sources:
  - path: https://www.sec.gov/search-filings/mutual-funds-search
    title: EDGAR system
  resources:
  - name: "currency_plot.ipynb"
    title: "currency_plot.ipynb"
    description: "Source code for the interactive dashboard."
    lastModified: 2025-02-12
    path: https://github.com/LennoxFang/HedgingPlot/archive/refs/heads/main.zip
  - name: "fwd_holding_merged_10q1-23q2.dta"
    title: "fwd_holding_merged_10q1-23q2.dta"
    description: "Main dataset for Hedging Position."
    lastModified: 2025-02-12
    path: https://github.com/LennoxFang/HedgingPlot/archive/refs/heads/main.zip
---

## Dashboard Features

- **Area Chart:** Shows the evolution of net positions over time for one or more selected currency derivatives.
- **Horizontal Bar Chart:** Displays net positions per currency derivatives for a selected quarter.


## Visual Output
<iframe 
  src="https://LennoxFang.github.io/HedgingPlot/area_chart.html" 
  width="1200" 
  height="1200" 
  frameborder="0">
</iframe>
<iframe src="https://LennoxFang.github.io/HedgingPlot/bar_chart.html" width="100%" height="1200" frameborder="0"></iframe>

*If the interactive graphs do not load, launch the interactive notebook in Binder:
https://mybinder.org/v2/gh/LennoxFang/HedgingPlot/d82983950f945d192ea751087ca13e69c8a64ffa?urlpath=lab%2Ftree%2Fcurrency_plot.ipynb

*Note:*  
- To view the interactive dashboard, you can run the provided Jupyter Notebook (`currency_plot.ipynb`) locally.
- Alternatively, you can deploy the app to a web server and provide a link for online interaction.

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/LennoxFang/HedgingPlot.git
   cd Hedging_Plot
