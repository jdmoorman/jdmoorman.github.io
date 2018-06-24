---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 1
topics:
  - Law of Total Probability
  - Bayes Formula
  - Conditional Probability
---

I flip a coin with probability \\(p\\) of heads until the first head occurs. Let \\(N\\) be the number of times I flip this coin. I then flip a coin with probability \\(q\\) of heads \\(N\\) times. Let \\(H\\) be the number of heads which occur with the second coin.

0. (<font color="green">Discussed</font>) Compute \\(P(N=n)\\)

1. (<font color="green">Discussed</font>) Compute \\(P(H=0)\\)

    * Hint: {{ page.topics[0] }}

1. (<font color="green">Discussed</font>) Compute \\(P(N=n\|H=0)\\)

    * Hint: {{ page.topics[1] }}

1. (<font color="green">Discussed</font>) Compute the distribution of \\[M(N) = \begin{cases}\frac{N}{2}, &\text{if } n \text{ is even}  \\\ \frac{N+1}{2}, &\text{if } n \text{ is odd} \end{cases}\\]

1. (<font color="green">Discussed</font>) Show memorylessness: \\(P(N=m+n\|N>m) = P(N=n)\\)

    * Hint: Use the definition of {{ page.topics[2] }}