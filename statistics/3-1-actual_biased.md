[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> 
import thinkstats2
import thinkplot

resp = nsfg.ReadFemResp()
df = resp['numkdhh']
pmf = thinkstats2.Pmf(df)
thinkplot.Hist(pmf, label = 'actual')
thinkplot.Config(xlabel = 'Kids per Household', ylabel = 'Pmf')
