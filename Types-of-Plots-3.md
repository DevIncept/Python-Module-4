# Contour graph
 <br>
 <ul>
 <li>
 Contour plots are aslo called Level Plots.
 </li>
 <li>
 Contour plots are a way to show a three-dimensional area on a two-dimensional plane.
 </li>
 <li>
 It shows the X and the Y variable on the Y axis , and the Z on the X axis.
 </li>
 <li>
 contour() function draws contour lines.
 </li>
 <li>
 contourf() function draws filled contours.
 </li>
 <li>
  Both functions require three parameters x,y and z.
 </li>
 </ul>
  Example:
  <br>
  17.
  <br>
 xlist = np.linspace(-10.0, 10.0, 100)
  <br>
  <br>
ylist = np.linspace(-5.0,53.0, 100)
  <br>
  <br>
X, Y = np.meshgrid(xlist, ylist)
  <br>
  <br>
Z = np.sqrt(X**2 + Y**2)
  <br>
  <br>
fig,ax=plt.subplots(1,1)
  <br>
  <br>
cp = ax.contourf(X, Y, Z)
  <br>
  <br>
fig.colorbar(cp) 
  <br>
  <br>
ax.set_title('Filled Contours Plot')
  <br>
  <br>
ax.set_ylabel('y (cm)')
  <br>
  <br>
plt.show()
  <br>
  Output:
  <br>
  <img src="https://user-images.githubusercontent.com/49331074/93021721-f4c25c80-f601-11ea-9cd2-1630625921d2.JPG">
  <br>
  <br>
  
# Box Plot
 <br>
 <ul>
 <li>A Box Plot is also known as Whisker plot
 </li>
 <li>
  In a box plot, we draw a box from the first quartile to the third quartile.
 </li>
 </ul>
 <br>
 Syntax:
 <br>
 matplotlib.pyplot.boxplot(x, notch=None, sym=None, vert=None, whis=None, positions=None, widths=None, patch_artist=None, bootstrap=None, usermedians=None, conf_intervals=None, meanline=None, showmeans=None, showcaps=None, showbox=None, showfliers=None, boxprops=None, labels=None, flierprops=None, medianprops=None, meanprops=None, capprops=None, whiskerprops=None, manage_ticks=True, autorange=False, zorder=None, data=None)
 <br>
 18.
 <br>
 np.random.seed(10) 
 <br>
 <br>
data = np.random.normal(50, 20, 100) 
<br>
<br>
plt.boxplot(data) 
<br>
<br>
plt.show() 
<br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93021879-0f490580-f603-11ea-836a-6db0f7eaba5e.JPG">
<br>
<br>
19.
<br>
np.random.seed(10) 
<br>
<br>
data_1 = np.random.normal(10, 10, 500) 
<br>
<br>
data_2 = np.random.normal(80, 20, 500) 
<br>
<br>
data_3 = np.random.normal(40, 30, 500) 
<br>
<br>
data_4 = np.random.normal(70, 40, 500) 
<br>
<br>
data = [data_1, data_2, data_3, data_4] 
<br>
<br>
fg = plt.figure(figsize =(10, 7)) 
<br>
<br>

axis = fg.add_axes([0, 0, 1, 1]) 
<br>
<br>
 
bp = axis.boxplot(data) 
<br>
<br>

plt.show() 
<br>
<br>
<img src="https://user-images.githubusercontent.com/49331074/93021880-1112c900-f603-11ea-961d-8e58ba60002c.JPG">
<br>
<br>

# Working with images
 <br>
 We need to import matplotlib.image for working with images.
 <br>
 <br>
 20.
 <br>
 import matplotlib.image as mpimg
 <br>
 img = mpimg.imread('DevIncept.png')
 <br>
 plt.imsave("logo.png", img, cmap = 'gray')
   <br>
 imgplot = plt.imshow(img)
   <br>
   <br>
   <img src="https://user-images.githubusercontent.com/49331074/93021955-9b5b2d00-f603-11ea-92f2-6ef151eeb689.JPG">
   <br>
   <br>
   <p>And we can continue playing with these!</p>
  
