---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 9
topics:
  - Compound Poisson Process
  - Thinning and Superposition
  - Miscillaneous Poisson Process
hidden: True
---

1. **{{ page.topics[0] }}**

    2. Let \\(X\_1, X\_2, \dots\\) be a sequence of i.i.d. random variables with mean \\(\mu\\) and variance \\(\sigma^2\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\). Define \\(S(t) = \sum\_{k=1}^{N(t)}X\_k\\).

        3. Compute \\(\mathbb{E}[S(t)]\\)

        3. Compute \\(\mathrm{Cov}(S(t\_1), S(t\_2))\\) for \\(t\_1 < t\_2\\)

        3. Compute \\(\mathrm{Var}(S(t))\\)

        3. Suppose the \\(X\_k\\) have MGF \\(M\_X(u)\\). Compute the MGF of \\(S(t)\\)

1. **{{ page.topics[1] }}**

    2. Let \\(N\_1(t)\\) and \\(N\_2(t)\\) be independent poisson processes with rates \\(\lambda\_1\\) and \\(\lambda\_2\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of \\(N\_1(t)\\) occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of \\(N\_2(t)\\).

    2. Let \\(N(t)\\) be a poisson process with rate \\(\lambda\\) and let each arrival of the process be identified as either type 1 with probability \\(p\\) or type 2 with probability \\(1-p\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of type 1 occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of type 2.

    2. Problem 2.48 from the textbook (2nd edition)

    2. Problem 2.52 from the textbook (2nd edition)

1. **{{ page.topics[2] }}**

    2. Let \\(X\_1, X\_2, \dots\overset{\mathrm{i.i.d}}{\sim} \mathrm{exp}(\lambda)\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\)

        3. Show the equality \\(P(\sum\_{i=1}^n X\_i \le t) = P(N(t) \ge n)\\)

        3. Find an analogous equality for \\(P(s \le \sum\_{i=1}^n X\_i \le t)\\)


