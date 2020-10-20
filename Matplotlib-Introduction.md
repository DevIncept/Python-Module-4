# **Matplotlib**

***What is matplotlib?***

Matplotlib is a library in python programming language.
We need to import this library using 'import' , before using it's features.

***Use of matplotlib:***

Matplotlib is a library in python. It helps in embedding plots.
Whenever we want to plot a agraph in python we use this library.

***Some types of graphs we can draw using matplotlib:***

1.Line plot<br>
2.Bar plot<br>
3.Histogram<br>
4.Scatter-plot<br>
5.Pie-chart<br>
6.Contour plot:<br>
7.Box plot<br>
8.Working with images<br>

First we need to install matplotlib using 'pip' command.<br>
Use the following command in the terminal:<br>
pip install matplotlib<br>

**Importing matplotlib:** <br>

import matplotlib.pyplot as plt<br>
This imports the matplotlib library to be used for plotting.<br>

<p>

<img src="https://user-images.githubusercontent.com/49331074/93016552-c3389980-f5df-11ea-9339-c2058cce1192.JPG">

## **Parts of a figure:**

### *Axes:*<br>
This is what you think of as 'a plot', it is the region of the image with the data space. 
A given figure can contain many Axes, but a given Axes object can only be in one Figure. 
The Axes contains two (or three in the case of 3D) Axis objects (be aware of the difference between Axes and Axis) 
which take care of the data limits (the data limits can also be controlled via the axes.Axes.set_xlim() and axes.Axes.set_ylim() methods). 
Each Axes has a title (set via set_title()), an x-label (set via set_xlabel()), and a y-label set via set_ylabel()).

The Axes class and its member functions are the primary entry point to working with the OO interface.

### *Axis:*<br>
These are the number-line-like objects.
They take care of setting the graph limits and generating the ticks (the marks on the axis) and ticklabels (strings labeling the ticks).
The location of the ticks is determined by a Locator object and the ticklabel strings are formatted by a Formatter.
The combination of the correct Locator and Formatter gives very fine control over the tick locations and labels.

### *Artist:*<br>
Basically everything you can see on the figure is an artist (even the Figure, Axes, and Axis objects).
This includes Text objects, Line2D objects, collections objects, Patch objects ... (you get the idea). 
When the figure is rendered, all of the artists are drawn to the canvas. Most Artists are tied to an Axes; 
such an Artist cannot be shared by multiple Axes, or moved from one to another.

</p>

<ul>
<li>An empty figure with no Axes</li>
</ul>

fig = plt.figure()
<br>
Output:<Figure size 432x288 with 0 Axes>
<br>

<ul>
<li>A figure with a single Axes</li>
</ul>

fig, ax = plt.subplots() 
<br>
Output:
<img src="https://user-images.githubusercontent.com/49331074/93016734-0e9f7780-f5e1-11ea-8943-86013a7c146c.JPG">
<br>
<p>
