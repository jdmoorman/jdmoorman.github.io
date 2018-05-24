---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 8
topics:
  - Exponential Distribution
  - Poisson Process Basics
---

1. **{{ page.topics[0] }}**

    2. Let \\(X \sim \mathrm{exp}(\lambda)\\).

        3. Find the distribution of \\(Y = \lceil X \rceil\\)

        3. Show that \\(X\\) and \\(Y\\) are both memoryless

        3. Find the distribution of \\(\beta X\\)

        3. Find the distribution of \\(e^{-X}\\)

    2. Let \\(U \sim \mathrm{uniform}[0,1]\\). Find the distribution of \\(-\alpha\log{U}\\)

    2. Let \\(X\_1, X\_2, \dots\overset{\mathrm{i.i.d}}{\sim} \mathrm{exp}(\lambda)\\)

        3. Suppose \\(N \sim \mathrm{geo}(p)\\). Find the distribution of \\(Z = \sum\_{i=1}^N X\_i\\).

        3. Find the distribution of \\(Q = \min(X\_1, X\_2, \dots X\_n)\\)

        3. Find the cumulative distribution of \\(V = \max(X\_1, X\_2, \dots X\_n)\\)

1. **{{ page.topics[1] }}**

    2. Let \\(N(t)\\) be a poisson process with rate \\(\lambda\\)

        3. Find the probability of no arrivals in \\((3,5]\\)

        3. Find the probability that there is exactly one arrival in each of the intervals: \\((0,1], (1,2], (2,3], (3,4]\\)

        3. Find the probability that there are two arrivals in \\((0,2]\\) and three arrivals in \\((1,4]\\)

        3. Find the covariance of \\(N(t\_1)\\) and \\(N(t\_2)\\) for \\(0 < t\_1 < t\_2\\)




