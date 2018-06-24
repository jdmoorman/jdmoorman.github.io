---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 9
topics:
  - Miscillaneous Poisson Process Problems
  - Compound Poisson Process
  - Thinning and Superposition
---

1. **{{ page.topics[0] }}**

    2. Let \\(X\_1, X\_2, \dots\overset{\mathrm{i.i.d}}{\sim} \mathrm{exp}(\lambda)\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\)

        3. Show the equality \\(P(\sum\_{i=1}^n X\_i \le t) = P(N(t) \ge n)\\)

        3. Find an analogous equality for \\(P(s \le \sum\_{i=1}^n X\_i \le t)\\)

            * (<font color="red">Answer</font>) \\(P(N(s) < n, N(t) \ge n)\\)

    2. \\(n+m\\) cars approach \\(n\\) toll booths \\((m < n)\\). The time taken for a car to pay its toll is exponentially distributed with rate \\(\lambda\\). When a toll booth becomes available, the next car in line fills it instantly if there are any cars waiting.

        3. What is the expected time before the first car exits the tolls?

            * (<font color="red">Answer</font>) \\(\frac{1}{n\lambda}\\)

        3. What is the expected time before the \\(m^\mathrm{th}\\) car exits the tolls?

            * (<font color="red">Answer</font>) \\(\frac{m}{n\lambda}\\)

        3. What is the expected time before the last car exits the tollbooths?

            * (<font color="blue">Solution</font>)

                * Let \\(\tau\_1, \tau\_2, \dots \tau\_{n+m}\\) be the times between successive cars exiting any of the tollbooths.

                * Then \\(\tau\_1\\), the time of the first car to exit any of the tolls, is the minimum of \\(n\\) exponential waiting times (for each of the tolls), and is therefore distributed exponential with parameter \\(n\lambda\\).

                * Likewise, \\(\tau\_2, \dots \tau\_{m+1}\\) are each the minimum of \\(n\\) exponential waiting times each (since the tolls are all occupied by cars until \\(m+1\\) cars have passed) and are therefore exponential with parameter \\(n\lambda\\).

                * After \\(m+1\\) cars have passed, there are more tollbooths than cars left, so there are no cars occupying some of the tollbooths. For this reason, \\(\tau\_{m+2}\\) is distributed exponentially with parameter \\((n-1)\lambda\\), \\(\tau\_{m+3}\\) is distributed exponentially with parameter \\((n-2)\lambda\\), and so on.

                * The quantity of interest is therefore \\[\begin{aligned}\mathbb{E}[\tau\_1 + \dots + \tau\_{m+n}] &= \mathbb{E}[\tau\_1] + \dots + \mathbb{E}[\tau\_{n+m}]\\\\&=\frac{m+1}{n\lambda} + \frac{1}{(n-1)\lambda} + \frac{1}{(n-2)\lambda} + \dots \frac{1}{\lambda}\end{aligned}\\]

        3. What is the probability that the \\((n+1)\\)st car to enter a toll exits before the first car to enter a toll?

            * (<font color="red">Answer</font>) \\(\frac{n-1}{n} \frac{1}{2}\\)

1. **{{ page.topics[1] }}**

    2. Let \\(X\_1, X\_2, \dots\\) be a sequence of i.i.d. random variables with mean \\(\mu\\) and variance \\(\sigma^2\\), and let \\(N(t)\\) be a poisson process with rate \\(\lambda\\) independent of all the \\(X\_k\\). Define \\(S(t) = \sum\_{k=1}^{N(t)}X\_k\\).

        3. Compute \\(\mathbb{E}[S(t)]\\)

            * (<font color="red">Answer</font>) \\(t \lambda \mu\\)

        3. Compute \\(\mathrm{Cov}(S(t\_1), S(t\_2))\\) for \\(t\_1 < t\_2\\)

            * (<font color="blue">Solution</font>)\\[\begin{aligned}\mathrm{Cov}(S(t\_1), S(t\_2)) &= \mathrm{Cov}(S(t\_1), S(t\_2) - S(t\_1) + S(t\_1))\\\\ &= \mathrm{Cov}(S(t\_1), S(t\_2) - S(t\_1)) + \mathrm{Var}(S(t\_1))\\\\&=\mathrm{Cov}(\sum\_{k=1}^{N(t\_1)}X\_k, \sum\_{k=N(t\_1)+1}^{N(t\_2)}X\_k) + \mathrm{Var}(S(t\_1))\\\\&=\mathrm{Var}(S(t\_1))\end{aligned}\\] Where the last equality comes from the independence of \\(X\_i\\) and \\(X\_j\\) for \\(i \neq j\\) and the fact that the sums \\(\sum\_{k=1}^{N(t\_1)}X\_k\\) and \\(\sum\_{k=N(t\_1)+1}^{N(t\_2)}X\_k\\) do not overlap in indices.

        3. Compute \\(\mathrm{Var}(S(t))\\)

            * (<font color="red">Answer</font>) \\(t\lambda(\sigma^2 + \mu^2)\\)

        3. Suppose the \\(X\_k\\) have MGF \\(M\_X(u)\\). Compute the MGF of \\(S(t)\\)

            * (<font color="red">Answer</font>) \\(e^{t\lambda(M\_X(u)-1)}\\)

1. **{{ page.topics[2] }}**

    2. Let \\(N\_1(t)\\) and \\(N\_2(t)\\) be independent poisson processes with rates \\(\lambda\_1\\) and \\(\lambda\_2\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of \\(N\_1(t)\\) occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of \\(N\_2(t)\\).

    2. Let \\(N(t)\\) be a poisson process with rate \\(\lambda\\) and let each arrival of the process be identified as either type 1 with probability \\(p\\) or type 2 with probability \\(1-p\\). Find the probability that the \\(m\_1^{\mathrm{th}}\\) arrival of type 1 occurs before the \\(m\_2^{\mathrm{th}}\\) arrival of type 2.

    2. \\(n+m\\) cars approach \\(n\\) toll booths \\((m < n)\\). The time taken for a car to pass through a toll booth is exponentially distributed with rate \\(\lambda\\). When a toll booth becomes available, a car fills it instantly if there are any cars waiting.

        3. (<font color="green">Discussed</font>) Describe the exits of first \\(m\\) cars from the toll booths as a superposition of poisson processes

        3. (<font color="green">Discussed</font>) What is the probability that the first car comes through the leftmost tollbooth?

        3. (<font color="green">Discussed</font>) What is the probability that all of the first \\(m\\) cars comes through the leftmost tollbooth?

        3. What is the probability that each of the first \\(m\\) cars go exit through a different tollbooth?

            * (<font color="red">Answer</font>) \\(\frac{n-1}{n}\frac{n-2}{n} \dots \frac{n-m+1}{n}\\)


