---
datapackage:
  title: Dataset of Currency Forward Position of U.S. international fixed income funds.
  description: >
    We present an interactive dashboard visualizing the net position of each currency derivative of mutual funds which is used to manage their currency exposures. 
    Here we collect the dataset of currency forward contracts used by U.S. international fixed-income funds.
  created: 2025-02-12
  updated: 2025-02-14
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
  sources:
  - path: https://www.sec.gov/search-filings/mutual-funds-search
    title: EDGAR system
  resources:
  - name: "CurrencyForward_plot.ipynb"
    title: "CurrencyForward_plot.ipynb"
    description: "Source code for the interactive dashboard."
    lastModified: 2025-02-12
    path: https://github.com/LennoxFang/HedgingPlot/archive/refs/heads/main.zip
  - name: "fwd_holding_merged_10q1-23q2.dta"
    title: "fwd_holding_merged_10q1-23q2.dta"
    description: "Main dataset for Hedging Position."
    lastModified: 2025-02-12
    path: https://github.com/LennoxFang/HedgingPlot/archive/refs/heads/main.zip
---
## Measurement of fund currency forwards
For each fund `i`, currency `c`, and date `t`, we define the Net Forward Sales (NFS) is calculated as follows:

<img width="1089" alt="de3e3f845c0ae0d45f58c1f5ef654c8" src="https://github.com/user-attachments/assets/e052d92f-6f66-40c2-892c-bbfb2e2a5642" />

We then aggregate the fund-level NFS position to form an overall metric `NFS_{c,t}` in order to capture the collective behavior of funds for each currency at given time `t`. Similarly, A positive `NFS_{c,t}` implies that funds are collectively hedging their exposure by selling forwards.
  
## Dashboard Features

- **Area Chart:** Shows the evolution of net forward sale positions over time for one or more selected currencies.
- **Horizontal Bar Chart:** Displays a broader picture of net forward sale positions per currency for a selected quarter.


## Visual Output
<iframe 
  src="https://LennoxFang.github.io/HedgingPlot/area_chart.html" 
  width="1200" 
  height="1200" 
  frameborder="0">
</iframe>
<iframe src="https://LennoxFang.github.io/HedgingPlot/bar_chart.html" width="100%" height="1200" frameborder="0"></iframe>

*More intuitively, you can launch the interactive notebook in Binder:
https://mybinder.org/v2/gh/LennoxFang/HedgingPlot/0b695102f616a3eb934de0fa995b4e10bac7e584?urlpath=lab%2Ftree%2FCurrencyForward_plot.ipynb

*Note:*  
- To view the interactive dashboard, you can run the provided Jupyter Notebook (`CurrencyForward_plot.ipynb`) locally.
- Alternatively, you can deploy the app to a web server and provide a link for online interaction.

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/LennoxFang/HedgingPlot.git
   cd HedgingPlot
