[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```
import scipy.stats
mu = 178
sigma = 7.7
male_heights_distribution = scipy.stats.norm(loc = mu, scale = sigma)
answer = male_heights_distribution.cdf(185.4) - male_heights_distribution.cdf(177.8)
print(answer)
```
