---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 6
topics:
  - Exit Distributions
  - Exit Times
---

1. **{{ page.topics[0] }}**

    2. A person is terminally ill. On a day when the person is awake, there is an 0.2 chance they will die overnight, and they are equally likely to be awake or unconscious the next day. On a day when the person is unconscious, there is an 0.2 chance they will be awake the next day, and they are equally likely to stay unconscious or die.

        3. Let \\(X\_n\\) be the person's state on day \\(n\\) (awake, unconscious, or dead). Show that \\((X\_n)\_{n\ge 0}\\) is a Markov chain. Find its transition matrix.

            * (<font color="red">Answer</font>) \\[\begin{matrix}& \mathbf A & \mathbf U & \mathbf D \cr \mathbf A & 0.4 & 0.4 & 0.2 \cr \mathbf U & 0.2 & 0.4 & 0.4 \cr \mathbf D & 0 & 0 & 1\end{matrix}\\]

        3. Compute the probability that the person spends at least one day awake before dying given that they are initially unconscious.

            * (<font color="red">Answer</font>) \\(\frac{0.2}{1-0.4} = \frac 1 3\\)

        3. Compute the expected number of days the person will spend awake before dying given that they are initially unconscious.

            * (<font color="red">Answer</font>) \\(\frac 5 7\\)

    2. In the Markov chain corresponding to the following transition matrix \\[\begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 \cr \mathbf 1 & 0.1 & 0.5 & 0.2 & 0.2 \cr \mathbf 2 & 0.2 & 0.4 & 0.4 & 0 \cr \mathbf 3 & 0 & 0.5 & 0.3 & 0.2 \cr \mathbf 4 & 0.5 & 0.5 & 0 & 0 \end{matrix}\\] compute the probability that the chain reaches state 1 before it reaches state 4 for each starting state.

        * (<font color="red">Answer</font>) Define \\(h(x)=P\_x(T\_1 < T\_4)\\). Then \\(h(1)=1\\), \\(h(4)=0\\), and \\[\begin{bmatrix}h(2) \cr h(3)\end{bmatrix} = \left(I - \begin{bmatrix}0.4 & 0.4 \cr 0.5 & 0.3\end{bmatrix}\right)^{-1}\begin{bmatrix}0.2 \cr 0\end{bmatrix}\\]

    2. (<font color="green">Discussed</font>) In the Markov chain corresponding to the following transition matrix \\[\begin{matrix} & \mathbf 1 & \mathbf 2 & \mathbf 3 & \mathbf 4 & \mathbf 5 \cr \mathbf 1 & 0.1 & 0.5 & 0.2 & 0.2 & 0 \cr \mathbf 2 & 0.4 & 0.2 & 0.3 & 0 & 0.1\cr \mathbf 3 & 0 & 0.5 & 0.3 & 0.2 & 0\cr \mathbf 4 & 0.2 & 0 & 0.5 & 0.1 & 0.2 \cr \mathbf 5 & 0.1 & 0.1 & 0.2 & 0.1 & 0.5 \end{matrix}\\] Compute the probability that the chain reaches states 1 or 2 before it reaches state 5 for each starting state.

1. **{{ page.topics[1] }}**

    2. In the Markov chain from 1.2 compute the expected time taken to reach state 4 from each of the other states.

        * (<font color="red">Answer</font>) \\(g(x)=\mathbb E\_x[T\_4]\\). Then \\(g(4)=0\\) and \\[\begin{bmatrix}g(1) \cr g(2) \cr g(3)\end{bmatrix} = \left(I - \begin{bmatrix}0.1 & 0.5 & 0.2 \cr 0.2 & 0.4 & 0.4 \cr 0 & 0.5 & 0.3 \end{bmatrix}\right)^{-1} \begin{bmatrix}1 \cr 1 \cr 1\end{bmatrix}\\]

    2. (<font color="green">Discussed</font>) In the Markov chain from 1.3 compute the expected time taken to reach either of states 2 or 5 from each of the other states. That is, \\(\mathbb E\_x[T]\\) where \\(T = \min \\{n \ge 0 \mid X\_n \in \\{2, 5\\}\\}\\)
