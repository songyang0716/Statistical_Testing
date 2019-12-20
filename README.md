# Some statistical testing methods that could be used in online experimentation #

### Repeated Measurement Experiments ###
 
1. Why do we use repeated measurements:
- Repeated measurement from a single subject provide more information than a single measurement obtained from a single subject, which improves the power of our study
- Each subject can serve as his/her own control (Diff-diff thought)
- We could separate the aging effects (changes over time effects, accumulative effects for online experimentation) 

2. Why difference-in-difference method could be wrong in experiment analysis<br/>
- One group pre-post test<br/>
- Two groups pre-post test<br/>

3. How to do the correct analysis for longitudinal dataset ?
- Repeated Measurement ANOVA - compound symmetry assumption possibly works for two data points scenarior, but not valid for more generalized repeated measurement 
- Paired T-Test for Two Time Points
   -- Solve the issue
- GEE Model - gee_simulation.Rmd
   -- It doesn't solve the issue, from the simulation result, we have seen ~ 0% type one error and low power
- Mixed Effects Model


### Cluster Randomized Experiment ###
1. The difference-in-means estimator is no longer unbiased


### Network Effects ###

