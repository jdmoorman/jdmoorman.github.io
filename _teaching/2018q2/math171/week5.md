---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 5
topics:
  - Reversibility/Detailed Balance Condition
  - Limiting Behavior
hidden: true
---

1. **{{ page.topics[0] }}**

    2. Suppose that \\(r\\) satisfies the detailed balance condition: \\(r\_i P\_\{ij\} = r\_j P\_\{ji\} \; \forall i, j\\). Show that \\(r\\) is stationary.

    2. Show that Ehrenfest's chain is reversible. \\[P(x,y)= \begin{cases}\frac{N-x}{N}, & \mathrm{if\ } y=x+1 \cr \frac{x}{N}, & \mathrm{if\ } y=x-1 \cr 0, & \mathrm{otherwise}\end{cases}\\]

    2. Consider the Markov chain \\(\\{X\_n:n \ge 0\\}\\) on \\(\mathcal{S} = \\{1, 2, \dots, N\\}\\) with a transition matrix of the form \\[P(x,x-1)=q(x), \; P(x,x)=r(x), \; P(x,x+1)=p(x)\\]

        3. Find conditions on \\(q, r, p\\) which guarantee the chain will be irreducible.

        3. Show the chain is reversible

        3. Find the stationary distribution, assuming the chain is irreducible

1. **{{ page.topics[1] }}**

    2. Consider Ehrenfest's chain \\(\\{X\_n:n \ge 0\\}\\) subject to the transition probabilities. \\[P(x,y)= \begin{cases}\frac{N-x}{N}, & \mathrm{if\ } y=x+1 \cr \frac{x}{N}, & \mathrm{if\ } y=x-1 \cr 0, & \mathrm{otherwise}\end{cases}\\]

        3. Compute the period \\(\\{X\_n:n \ge 0\\}\\)

        3. Show that \\(Y\_n=X\_{2n}\\) is a Markov chain. Is it irreducible?

        3. Consider \\(Y\_n=X\_{2n}\\) under the restriction \\(X\_0 \in \\{0,\ 2,\ \dots,\ 2\lfloor\frac{N}{2}\rfloor\\}\\). Compute its stationary distribution. Explain why \\(Y\_n\\) converges in distribution to the stationary distribution as \\(n \to \infty\\).

    2. Consider the Markov chain \\(\\{X\_n:n \ge 0\\}\\) on \\(\mathcal{S} = \\{1, 2, \dots, N\\}\\) with a transition matrix of the form \\[P(x,x-1)=q(x), \; P(x,x)=r(x), \; P(x,x+1)=p(x)\\]

        3. Find conditions on \\(q, r, p\\) which lead to a period of 2

        3. Suppose \\(q(x)=0\\). Find a formula for \\(\mathbb{E}\_x[N(y)]\\) for \\(x < y\\)

    2. Consider the Markov chain \\(\\{X\_n:n \ge 0\\}\\) on \\(\mathcal{S} = \\{1, 2, \dots, N\\}\\) with a transition matrix of the form \\[P(x,y)= \begin{cases}p, & \mathrm{if\ } y=x+1, \; x<N \cr 1-p, & \mathrm{if\ } x=0, \; y=0 \cr r & \mathrm{if\ } y = x, \; 0<y<N \cr q, & \mathrm{if\ } y=x-1, \; x>0 \cr 1-q, & \mathrm{if\ } x=N, \; y=N \cr 0, & \mathrm{otherwise}\end{cases}\\]

        3. Find a system of equations which could be solved to find \\(\mathbb{E}\_x[T\_N]\\) for any \\(x\\).

        3. Compute \\(\mathbb{E}\_x[T\_N]\\) when \\(r=0\\) and \\(q=1-p\\)