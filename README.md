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
1. Why do we use clustrer randomized experiment ?
- Sometimes, the unit randomization is infeasible or undesirable, the outcome measures are only available at the level of the cluster, or when unit interference with each other (Network Effects / Spillover Effects)

2. Issues/challenges with cluster randomized experiment
- The regular difference-in-means estimator is no longer unbiased (Mean of all samples in the treament cohort - mean of all samples in control cohort)

3. List of paper on this topic that I have read
- Unbiased Estimation of the Average Treatment Effect in Cluster-Randomized Experiments 

his paper explains why the regular difference-in-means estimator is biased, and it introduces an unbiased estimator for the average treatment effect of cluster randomized experiment
  
- Network A/B Testing: From Sampling to Estimation
- 

### Network Effects ###

