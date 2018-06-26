[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```
import nsfg
import thinkstats2
import thinkplot

df = nsfg.ReadFemPreg()

pregordr = df['pregordr']
preg_map = nsfg.MakePregMap(df)

preg = nsfg.ReadFemPreg()
live = preg[preg.outcome == 1]

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]

# Exercise 2.4
totalwgt_lb_diff = thinkstats2.CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
print(totalwgt_lb_diff)
```
