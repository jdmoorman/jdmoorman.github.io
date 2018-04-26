---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 4
topics:
  - Stationary Distributions
  - Reversibility/Detailed Balance Condition
  - Limiting Behavior
---

1. **{{ page.topics[0] }}**
    
    2. Compute any and all stationary distributions of \\[P = \begin{bmatrix} P\_1 & 0 & \dots & 0 \cr 0 & P\_2 & \dots & 0 \cr \vdots & \vdots & \ddots & \vdots \cr 0 & 0 & \dots & P\_k  \end{bmatrix}\\] where \\(P\_i\\) has a unique stationary distribution \\(\pi\_i\\) for each \\(i\\). If you claim \\(P\\) has a unique stationary distribution, please justify.

    2. (<font color="green">Discussed</font>) Expanding upon problem 2.1 in the week 3 handout, consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 & \mathbf 7 & \mathbf 8 \cr \mathbf 1 & 0.5 & 0 & 0.5 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 2 & 0.5 & 0.5 & 0 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 3 & 0 & 0 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \cr \mathbf 4 & 0 & 0 & 0.5 & 0 & 0.5 & 0 & 0 & 0 \cr \mathbf 5 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \cr \mathbf 6 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 7 & 0 & 0 & 0 & 0 & 0 & 0.5 & 0 & 0.5 \cr \mathbf 8 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \end{matrix}\\] Compute any and all stationary distributions. If you claim \\(P\\) has a unique stationary distribution, please justify.

1. **{{ page.topics[1] }}**
    
    2. Show that the Markov Chain defined by \\[P = \begin{bmatrix} 1-p & p \cr q & 1-q \end{bmatrix}\\] with \\(p,q > 0\\) will always satisfy detailed balance

    2. Does the following satisfy detailed balance? \\[P = \begin{bmatrix} 0.8 & 0.1 & 0.1 \cr 0.1 & 0.7 & 0.2 \cr 0.3 & 0.6 & 0.1 \end{bmatrix}\\]

    2. (<font color="green">Discussed</font>) Under what conditions on \\(p,q\\) will the following satisfy detailed balance? \\[P = \begin{bmatrix} 0 & 0.5 & 0.5 \cr p & 1-p-q & q \cr 0.4 & 0.6 & 0 \end{bmatrix}\\]


1. **{{ page.topics[2] }}**

    2. (<font color="green">Discussed</font>) Expanding upon problem 2.1 in the week 3 handout, consider the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 & \mathbf 6 & \mathbf 7 & \mathbf 8 \cr \mathbf 1 & 0.5 & 0 & 0.5 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 2 & 0.5 & 0.5 & 0 & 0 & 0 & 0 & 0 & 0 \cr \mathbf 3 & 0 & 0 & 0 & 0.5 & 0 & 0 & 0 & 0.5 \cr \mathbf 4 & 0 & 0 & 0.5 & 0 & 0.5 & 0 & 0 & 0 \cr \mathbf 5 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \cr \mathbf 6 & 0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \cr \mathbf 7 & 0 & 0 & 0 & 0 & 0 & 0.5 & 0 & 0.5 \cr \mathbf 8 & 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \end{matrix}\\] Compute \\(E\_2[N(6)]\\) and \\(E\_2[N(3)]\\)

    2. Compute \\(E\_1[N(2)]\\) and \\(E\_2[N(1)]\\) for the Markov chain defined by the following transition matrix: \\[P = \begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 \cr \mathbf 1 & 0.1 & 0.5 & 0.4 \cr \mathbf 2 & 0.4 & 0.2 & 0.4 \cr \mathbf 3 & 0 & 0 & 1 \end{matrix}\\]
