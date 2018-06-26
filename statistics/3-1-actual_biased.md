[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
import nsfg
import thinkstats2
import thinkplot

resp = nsfg.ReadFemResp()
numkdhh = resp['numkdhh']
numkdhh_pmf = thinkstats2.Pmf(numkdhh, label = 'actual')

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)

    for x, p in pmf.Items():
        new_pmf.Mult(x, x)

    new_pmf.Normalize()
    return new_pmf

numkdhh_biased_pmf = BiasPmf(numkdhh_pmf, label = 'observed')
thinkplot.PrePlot(2)
thinkplot.Pmfs([numkdhh_pmf, numkdhh_biased_pmf])
thinkplot.Show(xlabel = 'number of kids in a household', ylabel = 'PMF')
