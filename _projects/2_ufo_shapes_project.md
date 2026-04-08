---
name: UFO Visualization Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/hw5.png
description: Interactive visualizations of UFO sightings using Altair and Vega-Lite
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# UFO Sightings Visualizations

## Visualization 1: Distribution of UFO Shapes

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_chart1.json" style="width: 100%"></vegachart>

### Discussion
This chart shows the distribution of UFO sightings by reported shape. The most common shapes (light, triangle, and circle) appear much more often than the other shapes. The x-axis includes the categorical variable "shape," while the y-axis represents the count of sightings, and the bars are sorted in decreasing order to highlight the most frequent shapes. Data cleaning included removing rows that had missing shape values.

## Visualization 2: UFO Sightings Over Time by Shape
<vegachart schema-url="{{ site.baseurl }}/assets/json/hw5_chart2.json" style="width: 100%"></vegachart>

### Discussion
This chart shows the number of UFO sightings over time, while also allowing the user to filter the data by shape through an interactive dropdown menu. The visualization reveals how sightings have changed over time for different reported shapes. The x-axis includes the year of the sighting, while the y-axis represents the count of sightings. A line chart was used to make spotting patterns over time easier. Data transformations included extracting the year from the date variable, as well as removing rows that had missing shape values.

The interactive dropdown menu allows users to filter the visualization by selecting a specific shape they want to analyze and updating the chart to display only rows with the selected shape. It allows users to explore trends of different shapes efficiently.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/ufo-scrubbed-geocoded-time-standardized-00.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/petery22/petery22.github.io/blob/main/python_notebooks/hw5.ipynb" text="The Analysis" %}
</div>