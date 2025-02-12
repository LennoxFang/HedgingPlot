---
datapackage:
  title: "Plot of Hedging Position"
  description: "Interactive dashboard visualizing Hedging Position for multiple currencies and dates."
  created: 2025-02-12
  updated: 2025-02-12
  licenses:
    - path: "http://opendatacommons.org/licenses/pddl/"
      title: "Open Data Commons Public Domain Dedication and License v1.0"
  resources:
    - name: "currency_plot.ipynb"
      title: "currency_plot.ipynb"
      description: "Source code for the interactive dashboard."
      lastModified: 2025-02-12
      path: "https://github.com/LennoxFang/Hedging_Plot/archive/refs/heads/main.zip"
    - name: "fwd_holding_merged_10q1-23q2.dta"
      title: "fwd_holding_merged_10q1-23q2.dta"
      description: "Main dataset for Hedging Position."
      lastModified: 2025-02-12
      path: "https://github.com/LennoxFang/Hedging_Plot/archive/refs/heads/main.zip"
---

# Plot of Hedging Position

This repository contains an interactive dashboard built with Dash and Plotly that visualizes the hedging positions for various currencies.

## Dashboard Features

- **Horizontal Bar Chart:** Displays net positions per currency for a selected quarter.
- **Area Chart:** Shows the evolution of net positions over time for one or more selected currencies.

## Visual Output

Below is a screenshot of the dashboard output:

![Hedging Position Dashboard](dashboard_output.png)

*Note:*  
- To view the interactive dashboard, you can run the provided Jupyter Notebook (`currency_plot.ipynb`) locally.
- Alternatively, you can deploy the app to a web server and provide a link for online interaction.

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/LennoxFang/Hedging_Plot.git
   cd Hedging_Plot
