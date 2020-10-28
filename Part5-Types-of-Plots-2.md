# Histogram
 
 To draw a histogram we use, matplotlib.pyplot.hist.
 <br>
 Syntax:<br>
 matplotlib.pyplot.hist(x, bins=None, range=None, density=False, weights=None, cumulative=False, bottom=None, histtype='bar', align='mid', orientation='vertical', rwidth=None, log=False, color=None, label=None, stacked=False,  data=None, kwargs)
 <br>
 x: it takes an array or a sequence if array.
 <br>
 bins : bins defines the number of equal width bins in the the given range.
 <br>
 range:The lower and upper range of the bins.
 <br>
 density: It is a boolean value , and its default is False. If it is True,it draws and returns a probability density.
 <br>
 weights: array-like or None, default: None
 <br><br>
 **Steps to draw a histogram:**<br>
 Step 1: Install Matplotlib package<br>
 pip install matplotlib<br>
 Step 2: Collect data for the histogram<br>
 For example: We need age of hundred people<br>
 Step 3: Determine the number of bins<br>
 Step 4: Plot the histogram in Python using matplotlib<br><br>
 Examples<br>
 9.
 <br>y = [27,48,69,32,0] <br>
<br>
plt.hist(y) <br>
<br>

plt.show() <br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93020667-ecffb980-f5fb-11ea-87e0-40637120c0d9.JPG">
<br>

10.
<br>

y = [5,2,3,6,9] <br>
<br>
plt.hist(y) <br>
<br>
plt.show() <br>
<br>
Output:<br>
<img src="https://user-images.githubusercontent.com/49331074/93020931-a612c380-f5fd-11ea-9587-38e080228d26.JPG">
<br>
11.
<br>
ges = [2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40] <br>
<br>
range = (0, 100) <br>
<br>
bins = 10<br>
<br>
plt.hist(ages, bins, range, color = 'green',histtype = 'bar', rwidth = 0.8) <br>
<br>
plt.xlabel('Age group') <br>
<br>
plt.ylabel('No. of people affected by corona') <br>
<br>
plt.show()<br>

<br>

Output:<br>
<img src="https://user-images.githubusercontent.com/49331074/93020933-a8751d80-f5fd-11ea-8b24-00ff5650e123.JPG">
<br>
<nr>
 
# Scatter Plot
 
 To draw a histogram we use, matplotlib.pyplot.scatter.
 <br>
 Syntax:<br>
matplotlib.pyplot.scatter(x, y, s=None, c=None, marker=None, cmap=None, norm=None, vmin=None, vmax=None, alpha=None, linewidths=None, verts=<deprecated parameter>, edgecolors=None, *, plotnonfinite=False, data=None, kwargs)
<br>
  A scatter plot of x vs y.<br>
 <ul>
  <li>x, y:float or array-like</li>
  <li>s:float or array-like</li>
  <li>c:array-like or list of colours or colour</li>
  <li>The plot function will be faster for scatterplots where markers don't vary in size or color.</li>
 </ul>
 <br>
 Examples:<br>
12.
<br>
x = [5,2,3,6,9] <br>
 <br>
y = [27,48,69,32,100] <br>
<br>
plt.scatter(x,y) <br>
<br>
plt.show() <br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93021255-5e8d3700-f5ff-11ea-9fc5-9fa88a6f9672.JPG">
<br>
<br>
13.
 <br>
 x = [15,82,33,6,95] <br>
 <br>
y = [27,48,69,32,0] <br>
<br>
plt.scatter(x,y) <br>
<br>
plt.show() <br>
<br>
 <img src="https://user-images.githubusercontent.com/49331074/93021259-60ef9100-f5ff-11ea-8c05-710e0aca51b1.JPG">
<br>
<br>
 14.
 <br>
 x = [15,82,33,6,95,2,3,6,8,22,5,44,11,74,14,95,86,23] <br>
 <br>
y = [27,48,69,32,0,15,82,33,6,95,2,0,36,69,43,31,15,2] <br>
<br>
plt.scatter(x,y) <br>
<br>
plt.show() <br>
 <br>
 <br>
<img src="https://user-images.githubusercontent.com/49331074/93021260-62b95480-f5ff-11ea-870b-13e70e396975.JPG">
<br>
<br>
 15.<br>
 x = [15,82,33,6,95,2,3,6,8,22,5,44,11,74,14,95,86,23] <br>
 <br>
y = [27,48,69,32,0,15,82,33,6,95,2,0,36,69,43,31,15,2] <br><br>


plt.scatter(x, y, label= "stars", color= "red", marker= "*",* s=30) <br>
<br>
plt.show() <br>
<br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93021262-65b44500-f5ff-11ea-8033-b203e5472012.JPG">
<br>
This is how we change the label and colour of the marker.
<br>
<br>
# Pie-chart
<br>
A Pie Chart is a circular statistical plot that can display only one series of data.
<br>
Examples:<br>
16.
<br>

company = ['DevIncept', 'Adobe', 'Infosys', 'Amazon'] <br>
<br>
s = [8, 3, 4, 6] <br><br>

colors = ['r', 'y', 'g', 'b'] <br><br>

plt.pie(s, labels = company, colors=colors, startangle=90, shadow = True, explode = (0.2, 0, 0, 0), radius = 1.2, autopct = '%1.1f%%') <br><br>

plt.legend() <br><br>

plt.show() <br><br>

<img src="https://user-images.githubusercontent.com/49331074/93021413-0efb3b00-f600-11ea-85da-693367b718b2.JPG">
<br>
 17.
 <img src="https://user-images.githubusercontent.com/49331074/93021499-86c96580-f600-11ea-9de7-386c318d8a38.JPG">
 <br>
 <img src="https://user-images.githubusercontent.com/49331074/93021502-88932900-f600-11ea-92b9-5ddd5c8d6ad9.JPG">
 <br>
 
