---
name: Homework 8
tools: [Python, HTML, vega-lite]
image: assets/pngs/hw8.png
description: Homework 8 for IS 445
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 8
## Viz 1

<br>
<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>
<br>

### Line Chart:

#### Description:
This visualization is of the Mean of Square footage of the buildings constructed in a particular year. One can explore how the trend is moving as and when the years increase. We can observe that for olden times, propersties had a higher square footage, as there was a lot of land available and real estate market wasn’t properly established. However as we come towards recent years, the mean of square footage drastically decreases as demand for houses grow due to population increase as well as real estate market. One thing I would like to change if I had more time is the data, it requires cleaning, and pre-processing.

#### Design Choices:
- Vizualization done using vegalite then used Python+Altair to read the dictionary and convert it into a JSON file.
- **Encoding Types:**
  - X-axis represents the Year of Construction, chosen type : temporal.
  - Y-axis represents the Mean of Square footage of buildings., chosen type : quantitative.
<div class="left">
{% include elements/button.html link="https://github.com/JigyashuSaravta/JigyashuSaravta.github.io/blob/main/assets/json/chart1.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/JigyashuSaravta/JigyashuSaravta.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Notebook" %}
</div>

<br>
<br>
## Viz 2
<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart3.json" style="width: 100%"></vegachart>

<br>

### Pie Chart:

#### Description:
The pie chart shows distribution of the buildings based on its status, i.e In Use, Abandon, In Progress. for a more focused analysis.

#### Design Choices:
- Vizualization done using Python+Altair and then exported to JSON.
- **Encoding Types:**
  - Theta (angle) encodes the count of number of buildings of current status.
  - Color distinguishes different status of buildings.
  - Selected type is highlighted and others are greyed.
  - Tooltip includes count for additional information.

- **Color Scheme:**
  - A general color scheme is used to differentiate the status.

#### Data Transformations:
- The count of buuldings is calculated from the dataset.

#### Interactivity:
- Users can select specific status by clicking on the legend.
- Selection highlights chosen status, aiding in a more detailed analysis.
- Tooltip complements the selection interaction by showing the license type and count.
- To de-select, click on anything outside the legend.

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/JigyashuSaravta/JigyashuSaravta.github.io/blob/main/assets/json/chart3.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/JigyashuSaravta/JigyashuSaravta.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Notebook" %}
</div>
