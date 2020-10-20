 # **Line graph:**

Steps we follow to draw this graph:<br>

1.First, we define the x-axis and the y-axis values as lists.<br>
2.Using .plot() we plot the graph<br>
3.If we want , we can name the x-axis and the y-axis.<br>
4.We can also give a title to our graph.<br>
5.We use .show() to view our graph<br>

Example:<br>

1.<br>
<img src="https://user-images.githubusercontent.com/49331074/93016812-840b4800-f5e1-11ea-9f8e-7402fe761fd1.JPG">
<br>
<img src="https://user-images.githubusercontent.com/49331074/93016857-da788680-f5e1-11ea-857a-620a56479a08.JPG">
<br>
2.
<br><img src="https://user-images.githubusercontent.com/49331074/93016992-13652b00-f5e3-11ea-85a9-4f2ca39a5809.JPG">
<br>
<img src="https://user-images.githubusercontent.com/49331074/93016996-16601b80-f5e3-11ea-83c8-fc79e8652734.JPG">
<br>
## **Two or more lines on same graph:**

Example:<br>
3.
<br><img src="https://user-images.githubusercontent.com/49331074/93016936-799d7e00-f5e2-11ea-8264-15f716437089.JPG">
<br>
<img src="https://user-images.githubusercontent.com/49331074/93016954-98037980-f5e2-11ea-9744-a767f5b63902.JPG">
<br>
4.<br><img src="https://user-images.githubusercontent.com/49331074/93016955-99cd3d00-f5e2-11ea-8c43-0557e5dde87b.JPG">
<br>
<img src="https://user-images.githubusercontent.com/49331074/93016957-9cc82d80-f5e2-11ea-8861-e06c23985bc7.JPG">
<br>
Here, we plot two lines on same graph. We differentiate between them by giving them a name(label) which is passed as an argument of .plot() function.
The small rectangular box giving information about type of line and its color is called legend. We can add a legend to our plot using .legend() function.
<br>
5.<br>x = [1,2,3] <br>
y = [2,4,6] <br>
<br>
plt.plot(x, y, label = "line1") <br>
<br>
x1 = [1,2,3] <br>
y1 = [4,8,3] <br>
<br>
plt.plot(x1, y1, label = "line2") <br>
<br>
plt.xlabel('x-axis') <br>
<br>
plt.ylabel('y-axis') <br>
<br>
plt.title('Two lines on one graph') <br>
<br>
plt.legend() <br>
<br>
plt.show() <br>
<br>
Output:<br>
<img src="https://user-images.githubusercontent.com/49331074/93017128-d6e5ff00-f5e3-11ea-83ed-1200afbbc722.JPG">
<br>
<img src="https://user-images.githubusercontent.com/49331074/93017156-14e32300-f5e4-11ea-82d8-1aebed7a20ed.JPG">
</p>

# Bar Chart
To draw bar charts we use, plt.bar() function.<br>
We pass x-coordinates along with the required heights.
We can give names to x-axis coordinates.
<br>
Syntax:<br>
matplotlib.pyplot.bar(x, height, width=0.8, bottom=None, *, align='center', data=None, **kwargs)
<br>
<br>
<ul>
<li>The bars are at position x.</li>
<li>Height refers to the height of the bars.</li>
<li>We can pass the same height for all the bars , or , pass a list of different heights for each bars.</li>
<li>'align' is the alignment of the bars with the x-axis.</li>
<li>'center': Center the base on the x positions.</li>
<li>'edge': Align the left edges of the bars with the x positions.</li>
<li>We can add colours to the face of the bars as well as to the edges of the bars.</li>
<li>We can give linewidth of the bar.</li>
<li>If we put the linewidth to be 0 , then their won't be any bar edge.</li>
<li>We can provide tick_labels.</li>
<li>The default value of bottom is 0.</li>
</ul>
<br>
6.
<br>
x = [15,82,33,6,95] <br>
 <br>
y = [27,48,69,32,0] <br>
<br>
plt.bar(x,y) <br>
<br>
plt.show() <br>
<br>
Output:
<br>
<img src="https://user-images.githubusercontent.com/49331074/93017435-5ffe3580-f5e6-11ea-8631-56bf9c989323.JPG">
<br>
7.<br>
x = [5,2,3,6,9] <br>
 <br>
y = [27,48,69,32,100]  <br>
 <br>
plt.bar(x,y)  <br>
 <br>
plt.show()  <br>
<br>
Output: <br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93017495-d733c980-f5e6-11ea-815c-a50a9f5f33bf.JPG">
 <br>
 8.
 <br>
import matplotlib.pyplot as plt 
 <br>

 <br>
x = [1, 2, 3, 4, 5] 
 <br>
 <br>
 
h = [10, 24, 36, 40, 5] 
 <br>
 <br>

tick_label = ['one', 'two', 'three', 'four', 'five'] 
 <br>
 <br>

plt.bar(x, h, tick_label = tick_label, width = 0.6, color = ['blue', 'black']) 
 <br>
 <br>
 
plt.xlabel('x-axis') 
 <br>
 <br>

plt.ylabel('y-axis') 
 <br>
 <br>

plt.title('Bar graph!') 
 <br>
 <br>

plt.show() 
 <br>
 <br>
 Output:
 
 <br>
 <img src="https://user-images.githubusercontent.com/49331074/93017498-dd29aa80-f5e6-11ea-9445-570faf1ec794.JPG">
 
 <br>
 This is how we add colour to our bar graph.
 <br>
 
