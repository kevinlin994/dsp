[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
import numpy as np
import thinkstats2
import thinkplot
rand = np.random.random(1000)
pmf = thinkstats2.Pmf(rand)
thinkplot.Pmf(pmf, label = 'PMF of Random Numbers')
thinkplot.Config(xlabel = 'Random Numbers', ylabel = 'PMF')
```
![image](https://github.com/kevinlin994/dsp/blob/master/statistics/ch4ex2-1.png)

```python
cdf = thinkstats2.Cdf(rand)
thinkplot.Cdf(cdf, label = 'CDF of 1000 Random Numbers')
thinkplot.Config(xlabel = "Random Numbers", ylabel = 'CDF')
```
![image](https://github.com/kevinlin994/dsp/blob/master/statistics/chp4ex02-2.png)

This distribution is uniform.
