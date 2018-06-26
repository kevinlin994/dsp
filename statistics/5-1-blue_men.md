[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 
```python
import scipy.stats
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
a = dist.cdf(177.8)
b = dist.cdf(185.42)
b - a
```
34.27% of the U.S. Male population is the right height to join Blue Man Group.
