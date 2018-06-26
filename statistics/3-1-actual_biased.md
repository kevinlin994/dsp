[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> 
```python
import thinkplot
import thinkstats2
import nsfg
resp = nsfg.ReadFemResp()
df = resp['numkdhh']
pmf = thinkstats2.Pmf(df)
thinkplot.Hist(pmf, label = 'actual')
thinkplot.Config(xlabel = 'Kids per Household', ylabel = 'Pmf')
```
![image](https://github.com/kevinlin994/dsp/blob/master/statistics/ch3e1.png)

```python
observed = BiasPmf(pmf, 'observed')
thinkplot.Hist(observed, label = 'observed')
thinkplot.Config(xlabel = 'Kids per Household', ylabel = 'Pmf')
```
![image](https://github.com/kevinlin994/dsp/blob/master/statistics/ch3ex1-2.png)
```python
thinkplot.Pmfs([pmf, observed])
thinkplot.Config(xlabel='Kids per Household', ylabel='PMF')
print('actual mean = ' + str(pmf.Mean()), 'observed mean = ' + str(observed.Mean()))

```
![image](https://github.com/kevinlin994/dsp/blob/master/statistics/ch2ex1-3.png)
actual mean = 1.024205155043831 observed mean = 2.403679100664282
