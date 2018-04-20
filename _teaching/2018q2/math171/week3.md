---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 3
topics:
  - Stopping/Non-Stopping times
  - Classification of States
  - Stationary Distributions
---

1. **{{ page.topics[0] }}**

    2. Let \\(T\_1, T\_2\\) be stopping times for some Markov Chain \\(\\{X\_n:n \ge 0\\}\\). Which of the following will also necessarily be stopping times? Prove your claims.

        3. (<font color="green">Discussed</font>) \\(T\_3=5\\)
        3. \\(T\_4=T\_1 + T\_2 + 1\\)
        3. (<font color="green">Discussed</font>) \\(T\_5=T\_1 + T\_2 - 1\\)
            * (<font color="blue">Solution</font>) \\(T\_5\\) will not necessarily be a stopping time. Suppose \\(\\{X\_n:n \ge 0\\}\\) is the Markov Chain corresponding to the transition matrix \\[P = \begin{matrix} & \mathbf 0 & \mathbf 1 \cr \mathbf 0 & 1/2 & 1/2 \cr \mathbf 1 & 0 & 1 \end{matrix}\\] Suppose further that \\(T_1 = \min\\{n \ge 0: X\_n = \mathbf 0\\}\\) and \\(T_2 = \min\\{n \ge 0: X\_n = \mathbf 1\\}\\). If \\(T\_5\\) were a stopping time we would have \\(P(T\_5 = n \| X\_n = x\_n, \dots, X\_0=x\_0)\in \\{0, 1\\} \; \forall n\\). However, by definition of \\(T\_5\\)\\[P(T\_5 = 0 \| X\_0=\mathbf 0) = P(T\_1 + T\_2 = 1 \| X\_0=\mathbf 0)\\] by directly enumerating the possibilities we see \\[= P(T\_1 = 1, T\_2 = 0 \| X\_0=\mathbf 0) + P(T\_1 = 0, T\_2 = 1 \| X\_0=\mathbf 0)\\] and now using the Multiplication Rule \\[= P(T\_1 = 1 \| T\_2 = 0, X\_0=\mathbf 0)P(T\_2 = 0 \| X\_0=\mathbf 0)\\] \\[+ P(T\_2 = 1 \| T\_1 = 0, X\_0=\mathbf 0)P(T\_1 = 0 \| X\_0=\mathbf 0)\\] since \\(T\_1\\) and \\(T\_2\\) are stopping times this simplifies to \\[= P(T\_1 = 1 \| X\_0=\mathbf 0)P(T\_2 = 0 \| X\_0=\mathbf 0)\\]\\[ + P(T\_2 = 1 \| X\_0=\mathbf 0)P(T\_1 = 0 \| X\_0=\mathbf 0)\\] each term of which can be computed \\[=0 \cdot 0 + \frac 1 2 \cdot 1\\]\\[= \frac 1 2 \notin \\{0, 1\\}\\]


    2. (<font color="green">Discussed</font>) Solve problem 4(ii) on HW 2
        * (<font color="green">Discussed</font>) Show Lemma 1.3 from the textbook

1. **{{ page.topics[1] }}**

    2. Consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 & \mathbf 7 & \mathbf 8 \cr \mathbf 1 & 0.5 & 0 & 0.5 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 2 & 0.5 & 0.5 & 0 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 3 & 0 & 0 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \cr \mathbf 4 & 0 & 0 & 0.5 & 0 & 0.5 & 0 & 0 & 0 \cr \mathbf 5 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \cr \mathbf 6 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 7 & 0 & 0 & 0 & 0 & 0 & 0.5 & 0 & 0.5 \cr \mathbf 8 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \end{matrix}\\] Identify the transient and recurrent states, and the irreducible closed sets in the Markov chain. Give reasons for your answers.

    2. Consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 \cr \mathbf 1 & 0 & 0 & 1 & 0 & 0 & 0 \cr \mathbf 2 & 0 & 0 & 0 & 0 & 0 & 1 \cr \mathbf 3 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 4 & 0.25 & 0.25 & 0 & 0.5 & 0 & 0 \cr \mathbf 5 & 1 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 6 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \end{matrix}\\] Identify the transient and recurrent states, and the irreducible closed sets in the Markov chain. Give reasons for your answers.

1. **{{ page.topics[2] }}**

    Recall a stationary distribution is a vector \\(\pi\\) satisfying: \\[\sum \_i \pi(i)=1\\] \\[\pi(i)\ge 0, \quad \forall i\\] \\[\pi P = \pi\\]

    2. (<font color="green">Discussed</font>) Compute any and all stationary distributions of \\[P = \begin{bmatrix} 0 & 0 & 1 \cr 1 & 0 & 0 \cr 0 & 1 & 0 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Under what circumstances is the stationary distribution of \\[P = \begin{bmatrix} 1-r & 0 & r \cr p & 1-p & 0 \cr 0 & q & 1-q \end{bmatrix}\\] unique? Justify your answer. Compute the stationary distribution in this case.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} 1 & 0 \cr 0 & 1 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} P\_1 & 0 \cr 0 & P\_2 \end{bmatrix}\\] where \\(P\_1\\) has a unique stationary distribution \\(\pi\_1\\) and \\(P\_2\\) has a unique stationary distribution \\(\pi\_2\\). If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} 0 & p & 0 & 1-p \cr q & 0 & 1-q & 0 \cr 0 & 1-r & 0 & r \cr 1-s & 0 & s & 0 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.
