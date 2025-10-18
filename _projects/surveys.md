---
layout: default
title: "Workplace Surveys"
image: "/assets/projects/survey-thumbnail.png"
mathjax: true
layout: post
excerpt: "How do we properly analyze workplace surveys?"
date: 2025-10-18
---

## Part 1: Exact Interval in Workplace Well-being Surveys

A workplace well-being survey is repeated at one-year intervals at a workplace with $N$ employees. The purpose is to examine well-being among the current employees. The result for each year is expressed as an average (of respondents) and can range between 1 and 5.

Let $x_1$ be the measured average of respondents in year 1. Let $n_1$ be the number of respondents in year 1 (at most $N$). Let $x_2, n_2$ be the corresponding values for year 2. Let $y_1$ and $y_2$ be the average well-being score in year 1 and year 2 for the entire workplace, respectively. Note that these are unobserved since not everyone has responded.

Let us define $\Delta x = x_2 - x_1$. This is the observed difference (among respondents) from year 1 to year 2. Also define $\Delta y = y_2 - y_1$ as the actual difference from year 1 to year 2 for the entire workplace. Note that our best estimate of the latter difference—an estimate we denote $\widehat{\Delta y}$—is the measured difference from the well-being analysis:

$$\widehat{\Delta y} = \Delta x$$

### Lower Bound

A lower bound for the difference $\widehat{\Delta y}_{\text{lower}}$ can be found by imagining that employees who did not answer the survey in year 2 ($N - n_2$) would respond as **low** as possible (i.e., a score of 1), while employees who did not answer the survey in year 1 ($N - n_1$) would respond as **high** as possible (i.e., a score of 5). Formally:

$$\widehat{\Delta y}_{\text{lower}} = \frac{x_2 n_2 + (N-n_2) - (x_1 n_1 + 5(N - n_1))}{N}$$

### Upper Bound

Similarly, we can find an upper bound for the difference $\widehat{\Delta y}_{\text{upper}}$ by imagining that employees who did not answer the survey in year 2 ($N - n_2$) would respond as **high** as possible (i.e., a score of 5), while employees who did not answer the survey in year 1 ($N - n_1$) would respond as **low** as possible (i.e., a score of 1). Formally:

$$\widehat{\Delta y}_{\text{upper}} = \frac{x_2 n_2 + 5(N-n_2) - (x_1 n_1 + (N - n_1))}{N}$$

### Example

We examine a workplace with $N = 10$ employees. In the first year, $n_1 = 9$ respondents answered. In the second year, $n_2 = 8$ respondents answered. The annual averages were $x_1 = 4.1$ and $x_2 = 3.8$. Our estimate of the workplace's difference in well-being is $\widehat{\Delta y} = 3.8 - 4.1 = -0.3$.

The exact upper and lower bounds are:

$$\widehat{\Delta y}_{\text{lower}} = \frac{3.8 \times 8 + (10 - 8) - (4.1 \times 9 + 5 \times (10 - 9))}{10} = -0.95$$

$$\widehat{\Delta y}_{\text{upper}} = \frac{3.8 \times 8 + 5 \times (10 - 8) - (4.1 \times 9 + (10 - 9))}{10} = 0.25$$

---

## Part 2: Uncertainty in Finite Populations—Case Study: Well-being Survey

Suppose you conduct a well-being survey at a workplace. For the sake of example, let us assume there are $100$ employees.

The survey is based on a series of questions answered by $n < 100$ employees, and results in a total score $s_i$ for each employee $i$. Let us assume $n = 25$ employees have answered. A measure of well-being could be the average of all scores:

$$\hat{s} = \frac{1}{n} \sum_{i=1}^n s_i = \frac{1}{25} (s_1 + s_2 + \ldots + s_{25})$$

### Standard Error

To measure the uncertainty in our estimate, we can calculate the **standard error**:

$$\text{SE}(\hat{s}) = \frac{\hat{\sigma}}{\sqrt{n}} \sqrt{\frac{N-n}{N-1}}$$

where $N$ is the population size and $\hat{\sigma}$ is the sample standard deviation.

### Defining the Population

However, what is the population actually? Do we wish to

1. Understand well-being among the current employees? Then the population size is $N = 100$.
2. Understand well-being at the workplace (not just among current employees)? Then the population size is theoretically infinite, i.e., $N = \infty$.

In situation (1), the correction in the standard error equation becomes $\sqrt{\frac{100-25}{100-1}} = \frac{75}{99} \approx 0.75$. In situation (2), the correction becomes $\sqrt{\frac{\infty-25}{\infty-1}} = 1$, i.e., no correction. In situation (2), the ratio between the sample and population size thus has no bearing on the uncertainty. So if, for example, some employees fail to respond (assuming they don't fail to respond for reasons related to the survey), it makes no difference.

### Confidence Interval

In both situations, we can create a conservative 95% confidence interval for $s$ (the total score) using the formula:

$$\hat{s} \pm 2 \cdot \text{SE}(\hat{s})$$

### Example

We examine general well-being (situation 2) and survey $25$ employees. They score an average of $\hat{s} = 77$ (out of 100), and the spread in responses is $\hat{\sigma} = 20$. Then $\text{SE}(\hat{s}) = \frac{20}{\sqrt{25}} = 4$, and a confidence interval (CI) becomes:

$$\text{CI}: \quad 77 \pm 2 \times 4 = [69, 85]$$
