## Finding the largest audiences for NYC Artists

# Abstract

The problem we are addressing with this project is to locate the largest audience for an artist practicing in New York City. We use the MTA data provided from their
[website](http://web.mta.info/developers/turnstile.html) to serve as the foundation for answering this question. Using Exploratory Data Analysis and visual
representation of processed data, we provide key MTA stations of interest for an artist on their preferred day of performance.

# Design

Simply finding an audience is too broad of a problem. Instead we narrow our interests to areas that naturally see a lot of foot-traffic: New York City public
transit stops, especially subway stops. Since people exiting the subway will most likely leave the station right away, we needed to look at people entering the
stations as this implies that they are waiting for their train. During this wait is when an artist can garner the attention of the commuters. 

# Data

As stated in the abstract, we obtained the data from the MTA's website. We utilize three months of the most recently available data to provide the most accurate 
information. The raw dataset boasts around 2.5 million points of data stretching from the start of January to the end of March. The data includes features such 
as control area, location of turnstiles within a station, as well as cumulative exits and entries every four hours. However, we're only interested in the days, the 
number of entries, and the station names. Further cleaning of the data involved converting date and times as string values into pandas datetime values and converting
the cumulative entries into daily entries.

# Algorithms

Algorithms used were minimal in complexity. Some internally defined functions involved computation on Pandas series.

# Tools

We used Pandas for dataframe manipulation and cleaning, NumPy for more intensive numerical computations on individual series, then a combination of Matplotlib
and Seaborn for plotting.

# Communication

In this repository is a presentation of slides that walk through the process of identifying a problem, narrowing the scope, cleaning data, and presenting the 
visual information.
