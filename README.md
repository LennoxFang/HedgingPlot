---
datapackage:
  title: Plot of Hedging Position
  description: nteractive dashboard visualizing Hedging Position for multiple currencies and dates.
  created: 2025-02-12
  updated: 2025-02-12
  licenses:
  - path: http://opendatacommons.org/licenses/pddl/
    title: Open Data Commons Public Domain Dedication and License v1.0
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
# Plot of Hedging Position

This repository contains an interactive dashboard built with Dash and Plotly that visualizes the hedging positions for various currencies.

## Dashboard Features

- **Horizontal Bar Chart:** Displays net positions per currency for a selected quarter.
- **Area Chart:** Shows the evolution of net positions over time for one or more selected currencies.

## Visual Output
<iframe 
  src="https://LennoxFang.github.io/HedgingPlot/area_chart.html" 
  style="width:100%; min-width:1200px; height:900px; border:0;">
</iframe>
<iframe src="https://LennoxFang.github.io/HedgingPlot/bar_chart.html" width="100%" height="1200" frameborder="0"></iframe>
