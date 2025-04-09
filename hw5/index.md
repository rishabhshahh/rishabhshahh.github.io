---
layout: default
title: "HW5: Jekyll Webpage"
---

# HW5: License Data Visualizations

[The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv)  
[The Analysis](https://github.com/rishabhshahh/rishabhshahh.github.io/blob/main/HW_5_Rishabh_Shah.ipynb)

<iframe src="../plot1.html" width="700" height="400" style="border:none;"></iframe>

### Plot 1: Distribution of License Statuses by License Type

This bar chart visualizes the number of licenses issued across various professional categories in Illinois, such as cosmetology, dental, and private detective board certifications. Each bar is segmented by the current license status, showing whether it is active, not renewed, terminated, canceled, or otherwise inactive. This visualization provides an overview of which license types are most common and the current standing of professionals within each category.

To create this chart, I grouped the data by both `License Type` and `License Status` and then counted the number of records for each combination. I used a horizontal bar chart to accommodate longer category names and make comparisons clearer. The x-axis shows the number of licenses, and the y-axis lists license types in descending order. Color is used to indicate license status, making it easier to spot patterns between license activity and profession. Minimal data transformation was needed beyond grouping and sorting.

<iframe src="../plot2.html" width="700" height="400" style="border:none;"></iframe>

### Plot 2: Interactive View of License Types by County and Status

This interactive scatterplot displays the geographic distribution of license types across counties in Illinois, with color used to show the license status. Each point represents a unique combination of license type and county, which makes it easier to explore where specific professions are concentrated and how license status varies by location.

I filtered the dataset to remove any records with missing county data. The x-axis shows license types, the y-axis shows counties, and color encodes the license status. Circle marks are used to reduce clutter and overlap. The interactive features, including tooltips and zooming, allow users to explore the data in more detail. For example, you can quickly identify counties with a high number of active licenses for a specific profession or spot regions with more expired or canceled licenses. This interactivity encourages exploration and reveals relationships that may not be obvious in a static chart.

### Interactivity Discussion

The second plot includes interactivity through tooltips, panning, and zooming. When users hover over a data point, a tooltip displays the specific license type, county, and license status, which makes the plot more informative and engaging. The ability to zoom and pan allows users to explore dense areas of the chart more easily, especially when multiple license types overlap across counties. This interactivity improves clarity by enabling users to drill down into specific regions and categories without being overwhelmed by the full dataset at once. It transforms the chart from a static overview into a more dynamic, exploratory tool.
