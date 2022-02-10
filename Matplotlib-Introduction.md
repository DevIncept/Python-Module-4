# What is the Matplotlib? 

Matplotlib is an incredible tool for 2D arrays display in Python. Built on NumPy Array and designed to interact with a wider SciPy stack, Matplotlib is a multi-platform data visualization package. It was launched in 2002 by John Hunter. 

 

One of the major advantages is the fact that visual access in readily consumable images is possible to large volumes of data. There are various Matplotlib parts such as a line, a bar, a scatter, a histogram, etc. 

 

# Installation: - 

     python -mpip install -U matplotlib 

# Importing: - 

    from matplotlib import pyplot 

              or 

    import matplotlib.pyplot  



# Basic plots in Matplotlib: 

 

Matplotlib comes with a wide variety of plots. Plots helps to understand trends, patterns, and to make correlations. They’re typically instruments for reasoning about quantitative information. Some of the sample plots are covered here. 

 

 

 

1) Line plot: - 

        import matplotlib.pyplot as plt 

        import numpy as np 



        #Data for plotting 

        t = np.arange(0.0, 2.0, 0.01) 

        s = 1 + np.sin(2 * np.pi * t) 




        fig, ax = plt.subplots() 

        ax.plot(t, s) 

        ax.set(xlabel='time (s)', ylabel='voltage (mV)', title='Line Plot') 

        ax.grid() 

        plt.show() 

     <a href="https://imgbb.com/"><img src="https://i.ibb.co/RSLHkvM/Whats-App-Image-2021-07-13-at-12-12-17.jpg" alt="Whats-App-Image-2021-07-13-at-12-12-17" border="0"></a>

 

2)  Multiple subplots:- 

        import matplotlib.pyplot as plt 

        import numpy as np 




        x1 = np.linspace(0.0, 5.0) 

        x2 = np.linspace(0.0, 2.0) 




        y1 = np.cos(2 * np.pi * x1) * np.exp(-x1) 

        y2 = np.cos(2 * np.pi * x2) 




        fig, (ax1, ax2) = plt.subplots(2, 1) 

        fig.suptitle('Multiple subplots') 




        ax1.plot(x1, y1, 'o-') 

        ax1.set_ylabel('subplot 1') 




        ax2.plot(x2, y2, '.-') 

        ax2.set_xlabel('time (s)') 

        ax2.set_ylabel('subplot 2') 




        plt.show() 

 
      <a href="https://imgbb.com/"><img src="https://i.ibb.co/QC3L75x/Whats-App-Image-2021-07-13-at-12-12-31.jpg" alt="Whats-App-Image-2021-07-13-at-12-12-31" border="0"></a>

 

3) Histograms:- 

        import matplotlib.pyplot as plt 

        import numpy as np 




        np.random.seed(19680801) 




        # example data 

        mu = 100  # mean of distribution 

        sigma = 15  # standard deviation of distribution 

        x = mu + sigma * np.random.randn(437) 




        num_bins = 50 




        fig, ax = plt.subplots() 




        # the histogram of the data 

        n, bins, patches = ax.hist(x, num_bins, density=True) 




        # add a 'best fit' line 

        y = ((1 / (np.sqrt(2 * np.pi) * sigma)) * np.exp(-0.5 * (1 / sigma * 

                                                                 (bins - mu))**2)) 

        ax.plot(bins, y, '--') 

        ax.set_xlabel('xlabel') 

        ax.set_ylabel('ylabel') 

        ax.set_title(r'Histogram') 




        # Tweak spacing to prevent clipping of ylabel 

        fig.tight_layout() 

        plt.show() 


      <a href="https://imgbb.com/"><img src="https://i.ibb.co/nbGpVSh/Whats-App-Image-2021-07-13-at-12-12-46.jpg" alt="Whats-App-Image-2021-07-13-at-12-12-46" border="0"></a>
 

4)  Scatter-plot:- 

        import numpy as np 

        import matplotlib.pyplot as plt 

        import matplotlib.cbook as cbook 




        # Load a numpy record array from yahoo csv data with fields date, open, close, 

        # volume, adj_close from the mpl-data/example directory. The record array 

        # stores the date as an np.datetime64 with a day unit ('D') in the date column. 

        price_data = (cbook.get_sample_data( 

            'goog.npz', np_load=True)['price_data'].view(np.recarray)) 

        price_data = price_data[-250:]  # get the most recent 250 trading days 




        delta1 = np.diff(price_data.adj_close) / price_data.adj_close[:-1] 




        # Marker size in units of points^2 

        volume = (15 * price_data.volume[:-2] / price_data.volume[0])**2 

        close = 0.003 * price_data.close[:-2] / 0.003 * price_data.open[:-2] 




        fig, ax = plt.subplots() 

        ax.scatter(delta1[:-1], delta1[1:], c=close, s=volume, alpha=0.5) 




        ax.set_title('Volume and percent change') 




        ax.grid(True) 

        fig.tight_layout() 




        plt.show() 



       <a href="https://imgbb.com/"><img src="https://i.ibb.co/p0K1YDT/Whats-App-Image-2021-07-13-at-12-13-07.jpg" alt="Whats-App-Image-2021-07-13-at-12-13-07" border="0"></a>


5) Pie- Chart:- 

        import matplotlib.pyplot as plt 




        # Pie chart, where the slices will be ordered and plotted counter-clockwise: 

        labels = 'Frogs', 'Hogs', 'Dogs', 'Logs' 

        sizes = [15, 30, 45, 10] 

        explode = (0, 0.1, 0, 0)  # only "explode" the 2nd slice (i.e. 'Hogs') 




        fig1, ax1 = plt.subplots() 

        ax1.pie(sizes, 

                explode=explode, 

                labels=labels, 

                autopct='%1.1f%%', 

                shadow=True, 

                startangle=90) 

        ax1.axis('equal')  # Equal aspect ratio ensures that pie is drawn as a circle. 




        plt.show() 
        
        
        
      <a href="https://imgbb.com/"><img src="https://i.ibb.co/G9kMnQ7/Whats-App-Image-2021-07-13-at-12-13-18.jpg" alt="Whats-App-Image-2021-07-13-at-12-13-18" border="0"></a>

 

 
 


There are some basic plots in the matplotlib library. If you want to learn more deeply then please check out the matplotlib documentation link:- https://matplotlib.org/stable/contents.html   

 

 

 