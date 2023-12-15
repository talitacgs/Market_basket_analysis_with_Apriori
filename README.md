<h1> Market Basket Analysis using Apriori Algorithm</h1>

<h2>Objective </h2>
Using the Apriori algorithm and association rules to identify frequent itens

<h2>Skills </h2>

* Explore Data Visualization;
* Apriori algorithm;
* Association Rules;

<h2>Data Source </h2>

[Groceries Dataset](https://www.kaggle.com/datasets/heeraldedhia/groceries-dataset) from Kaggle

<h2>Tools and Technologies </h2>

1. Google Colab;
2. Python 3.10.12;
3. Pandas 1.5.3;
4. mlxtend 0.22.0;


<h2>Dependencies </h2>
For the project, libraries can be divided into two types:

1. General

```
import pandas as pd
```

2. Model Building

```
from mlxtend.frequent_patterns import association_rules, apriori
```

<h2>Data Cleaning</h2>

Steps:

* Adjust data type using `.to_datetime()` and `.astype(str)` from `pandas`;
* Rename column using `.rename()` from `pandas`;

<h2>Data Pre Processing</h2>

Steps:
* Detecting Weekday using `.dt.weekday()` from `pandas` and replace the output for day name;
* Making a matrice with `.pivot_table()`

<h2>Data Visualization</h2>

ASAP ... 🚧👩‍💻

<h2>Data Building</h2>

* `apriori()` is a Naive Bayes Gaussian model;
  * min_support:
* `association_rules()` 
  * metric:
  * min_threshold:

<h2>Results and Output</h2>

Arranging the data from highest to lowest with respect to 'confidence' we observed that people who bought domestic eggs and meat, also bought meat in 1% of cases with a confidence level of 78%

But let's understand better all output:

* Antecedents / Consequents: They represents the sets of items in antecedent and consequence of each rule, respectively;
* Confidence: Indicates the probability of finding the consequence in a transaction that already contains the antecedent;
* Lift: Measures how much more likely the consequence is given that the advance occured compared to its expected probability if the antecedent and consequence were independent;
* Leverage: Measures the difference between the actual joint occurence and the expected occurence of they were independent;
* Conviction: Measures the dependence of a consequence on antecedent.
* Zhang's metric: Measure that takes into account both association and dissociation between items in an association rule. This can be useful in scenarios where not only the presence but also the absence of certain items is relevant to the interpretation of the rules.


<h2>References</h2>

* [mlxtend library](https://rasbt.github.io/mlxtend/user_guide/frequent_patterns/association_rules/)
* chatgpt
* [market basket analysis implementation in R](https://www.kaggle.com/code/heeraldedhia/market-basket-analysis-using-apriori-algorithm)
