# linegraph package

This package allows to produce a well-formatted and well-labeled line graph for time series using the plotly library.

# Files

**Preparedata.py:

Class PrepareData

  Attributes:
      * x - first column of dataset representing time (year, date, month). 
      * y - second column of the dataset representing the data series.
   Methods:
      * calculate_average() - computes the mean of the dataset (y column)
      * percentage_change() - computes the percentage change from the previous year
      * read_data_file(file_name) - uploads data from txt, csv

**Linegraph.py:

Class LineGraph(ReadData)

	Attributes:
    	* x_label - x-axis label
        * y_label - y-axis label
        * title - figure title
        * text - short description of main highlights in the graph
        * lab_axes_dict - dictionary for labeling axis
        * lab_title_dict - dictonary for labeling title
        * layout - set layout of all the annotations
	Methods:
    	* line_plot() - plot a line graph for the time series, the average line, all the annotations including a box 					containig the main highlights
        * save_fig(name) - save plot as png
    

# Installation

The following packages are required:
* plotly
* pandas
* numpy