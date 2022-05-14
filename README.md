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

  
