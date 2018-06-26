[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
import random
import thinkstats2

# Exercise 4.2
rand_list = [random.random() for i in range(0, 1000, 1)]
rand_pmf = thinkstats2.Pmf(rand_list)

thinkplot.Pmf(rand_pmf)
thinkplot.Show(xlabel = 'random number', ylabel = 'PMF')

rand_cdf = thinkstats2.Cdf(rand_list, label = 'random number CDF')

thinkplot.Cdf(rand_cdf)
thinkplot.Show(xlabel = 'random numbers', ylabel = 'CDF')
```
