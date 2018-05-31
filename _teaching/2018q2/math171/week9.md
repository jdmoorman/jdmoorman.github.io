---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 9
topics:
  - Miscillaneous Poisson Process Problems
  - Compound Poisson Process
  - Thinning and Superposition
hidden: True
---

1. **{{ page.topics[0] }}**

    2. Let \\(X\_1, X\_2, \dots\overset{\mathrm{i.i.d}}{\sim} \mathrm{exp}(\lambda)\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\)

        3. Show the equality \\(P(\sum\_{i=1}^n X\_i \le t) = P(N(t) \ge n)\\)

        3. Find an analogous equality for \\(P(s \le \sum\_{i=1}^n X\_i \le t)\\)

    2. \\(n+m\\) cars approach \\(n\\) toll booths \\((m < n)\\). The time taken for a car to pass through a toll booth is exponentially distributed with rate \\(\lambda\\). When a toll booth becomes available, a car fills it instantly if there are any cars waiting.

        3. What is the expected time before the first car exits the tolls?

        3. What is the expected time before the \\(m^\mathrm{th}\\) car exits the tolls?

        3. What is the expected time before the last car exits the tollbooths?

1. **{{ page.topics[1] }}**

    2. Let \\(X\_1, X\_2, \dots\\) be a sequence of i.i.d. random variables with mean \\(\mu\\) and variance \\(\sigma^2\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\). Define \\(S(t) = \sum\_{k=1}^{N(t)}X\_k\\).

        3. Compute \\(\mathbb{E}[S(t)]\\)

        3. Compute \\(\mathrm{Cov}(S(t\_1), S(t\_2))\\) for \\(t\_1 < t\_2\\)

        3. Compute \\(\mathrm{Var}(S(t))\\)

        3. Suppose the \\(X\_k\\) have MGF \\(M\_X(u)\\). Compute the MGF of \\(S(t)\\)

1. **{{ page.topics[2] }}**

    2. Let \\(N\_1(t)\\) and \\(N\_2(t)\\) be independent poisson processes with rates \\(\lambda\_1\\) and \\(\lambda\_2\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of \\(N\_1(t)\\) occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of \\(N\_2(t)\\).

    2. Let \\(N(t)\\) be a poisson process with rate \\(\lambda\\) and let each arrival of the process be identified as either type 1 with probability \\(p\\) or type 2 with probability \\(1-p\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of type 1 occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of type 2.

    2. \\(n+m\\) cars approach \\(n\\) toll booths \\((m < n)\\). The time taken for a car to pass through a toll booth is exponentially distributed with rate \\(\lambda\\). When a toll booth becomes available, a car fills it instantly if there are any cars waiting.

        3. Describe the exits of first \\(m\\) cars from the toll booths as a superposition of poisson processes

        3. What is the probability that the first car comes through the leftmost tollbooth?

        3. What is the probability that all of the first \\(m\\) cars comes through the leftmost tollbooth?

        3. What is the probability that each of the first \\(m\\) cars go exit through a different tollbooth?


