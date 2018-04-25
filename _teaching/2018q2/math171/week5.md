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

1. **{{ page.topics[1] }}**

    2. Consider Ehrenfest's chain \\(\\{X\_n:n \ge 0\\}\\) subject to the transition probabilities. \\[P(x,y)= \begin{cases}\frac{N-x}{N}, & \mathrm{if\ } y=x+1 \cr \frac{x}{N}, & \mathrm{if\ } y=x-1 \cr 0, & \mathrm{otherwise}\end{cases}\\]

        3. Compute the period \\(\\{X\_n:n \ge 0\\}\\)

        3. Show that \\(Y\_n=X\_{2n}\\) Markov chain. Is it irreducible?

        3. Consider \\(Y\_n=X\_{2n}\\) under the restriction \\(X\_0 \in \\{0,\ 2,\ \dots,\ 2\lfloor\frac{N}{2}\rfloor\\}\\). Compute its stationary distribution. Explain why \\(Y\_n\\) converges in distribution to the stationary distribution as \\(n \to \infty\\).
