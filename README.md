# ThinkStats2 Note
## Chapter 1. Exploratory data analysis
### 1.1 A statistical approach
1. Data collection
2. Descriptive statistics
3. Exploratory data analysis
4. Estimation
5. Hypothesis testing
- By performing these steps with care to avoid pitfalls, we can reach conclusions
that are more justifiable and more likely to be correct
### 1.5 Variables
- If you read the codebook carefully, you will see that many of the variables
are recodes, which means that they are not part of the raw data collected
by the survey; they are calculated using the raw data.
- Recodes are often based on logic that checks the consistency and accuracy of
the data. In general it is a good idea to use recodes when they are available,
unless there is a compelling reason to process the raw data yourself
### 1.6 Transformation
- data cleaning
- Special values encoded as numbers are dangerous because if they are not
handled properly, so replaces them with nan “not a number.” is a good method.
### 1.7 Validation
- When data is exported from one software environment and imported into
another, errors might be introduced.
- If you take time to validate the data, you can save time
later and avoid errors

- Method: compute basic statistics and compare them
with published results
  - like... df.value_counts(sort=False)
### 1.8 Interpretation
- To work with data effectively, you have to think on two levels at the same
time: the level of statistics and the level of context.
## Chapter 2. Distribution
### 2.5 Outliers
- The best way to handle outliers depends on “domain knowledge”
### 2.6 First Babies
- Histograms are useful because they make the most frequent values immediately apparent. But they are not the best choice for comparing two distributions. In this example, there are fewer “first babies” than “others,” so some
of the apparent differences in the histograms are due to sample sizes. In the
next chapter we address this problem using probability mass functions.
### 2.7 Summarizing distributions
- A histogram is a complete description of the distribution of a sample; that is,
given a histogram, we could reconstruct the values in the sample (although
not their order).
  - central tendency: Do the values tend to cluster around a particular
point?
  - modes: Is there more than one cluster?
  - spread: How much variability is there in the values?
  - tails: How quickly do the probabilities drop off as we move away from
the modes?
  - outliers: Are there extreme values far from the modes?
> Statistics designed to answer these questions are called <b>summary statistics</b>.
- For some data, mean is a good description of a set of values.
### 2.8 Variance
- If there is no single number that summarizes pumpkin weights, we can do a
little better with two numbers: mean and variance.
> For all live births, the mean pregnancy length is 38.6 weeks, the standard
deviation is 2.7 weeks, which means we should expect deviations of 2-3 weeks
to be common.

> Variance of pregnancy length is 7.3, which is hard to interpret, especially
since the units are weeks2
, or <b>“square weeks.” Variance is useful in some
calculations, but it is not a good summary statistic</b>.
  
### 2.9 Effect size
- An effect size is a summary statistic intended to describe (wait for it) the
size of an effect. For example, to describe the difference between two groups,
one obvious choice is the difference in the means.
- That's say that use mean, var, std to compare the difference between data.

### 2.10 Reporting results
- We have seen several ways to describe the difference in pregnancy length (if
there is one) between first babies and others. How should we report these
results?
> The answer depends on who is asking the question.

### Exercises
- Effect Size: 
  - for sample size, how many sample's size is enough to have credibility.
  - less effect size --> need more samples to have credibility and reliablity.
  - https://ithelp.ithome.com.tw/articles/10229159

## Chapter 3. Probability mass functions
