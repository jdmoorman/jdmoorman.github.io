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

        3. \\(T\_3=5\\)
        3. \\(T\_4=T\_1 + T\_2 + 1\\)
        3. \\(T\_5=T\_1 + T\_2 - 1\\)

    2. Solve problem 4(ii) on HW 2
        * Show Lemma 1.3 from the textbook

1. **{{ page.topics[1] }}**

    2. Consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 & \mathbf 7 & \mathbf 8 \cr \mathbf 1 & 0.5 & 0 & 0.5 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 2 & 0.5 & 0.5 & 0 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 3 & 0 & 0 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \cr \mathbf 4 & 0 & 0 & 0.5 & 0 & 0.5 & 0 & 0 & 0 \cr \mathbf 5 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \cr \mathbf 6 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 7 & 0 & 0 & 0 & 0 & 0 & 0.5 & 0 & 0.5 \cr \mathbf 8 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \end{matrix}\\] Identify the transient and recurrent states, and the irreducible closed sets in the Markov chain. Give reasons for your answers.

    2. Consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 \cr \mathbf 1 & 0 & 0 & 1 & 0 & 0 & 0 \cr \mathbf 2 & 0 & 0 & 0 & 0 & 0 & 1 \cr \mathbf 3 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 4 & 0.25 & 0.25 & 0 & 0.5 & 0 & 0 \cr \mathbf 5 & 1 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 6 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \end{matrix}\\] Identify the transient and recurrent states, and the irreducible closed sets in the Markov chain. Give reasons for your answers.

1. **{{ page.topics[2] }}**

    Recall a stationary distribution is a vector \\(\pi\\) satisfying: \\[\sum \_i \pi(i)=1\\] \\[\pi(i)\ge 0, \quad \forall i\\] \\[\pi P = \pi\\]

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} 0 & 0 & 1 \cr 1 & 0 & 0 \cr 0 & 1 & 0 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Under what circumstances is the stationary distribution of \\[P = \begin{bmatrix} 1-r & 0 & r \cr p & 1-p & 0 \cr 0 & q & 1-q \end{bmatrix}\\] unique? Justify your answer. Compute the stationary distribution in this case.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} 1 & 0 \cr 0 & 1 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} P\_1 & 0 \cr 0 & P\_2 \end{bmatrix}\\] where \\(P\_1\\) has a unique stationary distribution \\(\pi\_1\\) and \\(P\_2\\) has a unique stationary distribution \\(\pi\_2\\). If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} 0 & p & 0 & 1-p \cr q & 0 & 1-q & 0 \cr 0 & 1-r & 0 & r \cr 1-s & 0 & s & 0 \end{bmatrix}\\] If you claim \\(P\\) has a unique stationary distribution, please justify.
