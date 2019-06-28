---
title: Graph visualization
list_title: Graph
list_image: /img/2-0-visualizations-line-graph-example.png
description: >
  The Graph view lets you select from multiple graph types such as line graphs and bar graphs *(Coming)*.
weight: 201
menu:
  v2_0:
    name: Graph
    parent: Visualization types
---

The Graph visualization provides several types of graphs, each configured through
the [Graph options](#graph-options).

{{< img-hd src="/img/2-0-visualizations-line-graph-example.png" alt="Line Graph example" />}}

Select the **Graph** option from the visualization dropdown in the upper right.

## Graph behavior
The Graph visualization color codes each table (or series) in the queried data set.
When multiple series are present, it automatically assigns colors based on the selected [Line Colors option](#options).

When using a line graph, all points within a single table are connected. When multiple series are present, it automatically assigns colors based on the selected [Line Colors option](#options).

## Graph controls
To view **Graph** controls, click the settings icon ({{< icon "gear" >}}) next
to the visualization dropdown in the upper right.

###### Data
- **X Column**: Select a column to display on the x-axis.
- **Y Column**: Select a column to display on the y-axis.

###### Options
- **Interpolation**: Select from the following options:
  - **Line**: Display a time series in a line graph
  - **Smooth**: Display a time series in a line graph with smooth point interpolation.
  - **Step**: Display a time series in a staircase graph.
  <!-- - **Bar**: Display the specified time series using a bar chart. -->
  <!-- - **Stacked**: Display multiple time series bars as segments stacked on top of each other. -->
- **Line Colors**: Select a color scheme to use for your graph.
- **Shade Area Below Lines**: Shade in the area below the graph lines.

###### Y Axis
- **Y Axis Label**: Label for the y-axis.
- **Y Tick Prefix**: Prefix to be added to y-value.
- **Y Tick Suffix**: Suffix to be added to y-value.
- **Y Axis Domain**: The y-axis value range.
  - **Auto**: Automatically determine the value range based on values in the data set.
  - **Custom**: Manually specify the value range of the y-axis.
      - **Min**: Minimum y-axis value.
      - **Max**: Maximum y-axis value.

## Graph Examples

##### Graph with linear interpolation
{{< img-hd src="/img/2-0-visualizations-line-graph-example.png" alt="Line Graph example" />}}

##### Graph with smooth interpolation
{{< img-hd src="/img/2-0-visualizations-line-graph-smooth-example.png" alt="Step-Plot Graph example" />}}

##### Graph with step interpolation
{{< img-hd src="/img/2-0-visualizations-line-graph-step-example.png" alt="Step-Plot Graph example" />}}

<!-- ##### Stacked Graph example
{{< img-hd src="/img/2-0-visualizations-stacked-graph-example.png" alt="Stacked Graph example" />}} -->

<!-- ##### Bar Graph example
{{< img-hd src="/img/2-0-visualizations-bar-graph-example.png" alt="Bar Graph example" />}} -->