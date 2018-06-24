---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 2
topics:
  - Markov/Non-Markov Chains
  - Stopping/Non-Stopping Times
  - Linear Algebra
---

1. **{{ page.topics[0] }}**

    2. (<font color="green">Discussed</font>) Example 1.2 from the book (Ehrenfest Chain)

    2. (<font color="green">Discussed</font>) At \\(t=0\\) an urn contains \\(N\\) balls, \\(M\\) of which are red, \\(N-M\\) of which are green. Each day (\\(t = 1, 2, \dots\\)) a ball is drawn without replacement. Let \\(X\_n\\) be the color of the ball drawn at \\(t=n\\). Is \\(\\{X\_n:N \ge n \ge 1\\}\\) a Markov Chain? Prove your claim.

    2. Example 1.6 from the book (Inventory Chain)

    2. Let \\(\\{X\_n:n \ge 0\\}\\) be a Markov Chain on the state space \\(\mathcal{S}=\\{0, 1, 2\\}\\). Define \\[Y\_n=I\_{\[X\_n \ge 1\]} = \begin{cases}1 &\text{if } X\_n =1,2  \cr 0 &\text{if } X\_n = 0\end{cases}\\] Under what circumstances, if any, is \\(\\{Y\_n:n \ge 0\\}\\) a Markov Chain?

1. **{{ page.topics[1] }}**

    2. Let \\(\\{X\_n:n \ge 0\\}\\) be a Markov Chain. Which of the following will necessarily be stopping times? Prove your claims.

        3. (<font color="green">Discussed</font>) \\(T=\min\\{n \ge 0: X\_n = x\\}\\)
        3. (<font color="green">Discussed</font>) \\(T=\max\\{n \ge 0: X\_n = x\\}\\)
        3. \\(T=\min\\{n \ge 0: X\_n = X\_{n-1}\\}\\)
        3. (<font color="green">Discussed</font>) \\(T=\min\\{n \ge 0: X\_{n+1} = X\_{n}\\}\\)

    2. Let \\(T\_1, T\_2\\) be stopping times for some Markov Chain \\(\\{X\_n:n \ge 0\\}\\). Which of the following will also necessarily be stopping times? Prove your claims.

        3. \\(T\_1 + T\_2\\)

            * (<font color="red">Answer</font>) Yes

        3. \\(T\_1 - T\_2\\)

            * (<font color="red">Answer</font>) No

        3. \\(\min(T\_1, T\_2)\\)

            * (<font color="red">Answer</font>) Yes

        3. \\(\max(T\_1, T\_2)\\)

            * (<font color="red">Answer</font>) Yes

1. **{{ page.topics[2] }}**

	2. Compute or write down the inverse of the matrix \\[A = \begin{bmatrix} a & b \cr c & d \end{bmatrix}\\]

        * (<font color="red">Answer</font>) \\[\frac{1}{ad-bc}\begin{bmatrix}d & -b \\\\ -c a\end{bmatrix}\\]

	2. Under what circumstances is the following matrix invertible? Under these circumstances, compute its inverse. \\[A = \begin{bmatrix} a & 0 & 0 \cr b & c & 0 \cr 0 & d & e \end{bmatrix}\\]

        * (<font color="red">Answer</font>) \\(ace \neq 0\\)

    2. Compute the left eigenvector of \\[P = \begin{bmatrix} 1-r & 0 & r \cr p & 1-p & 0 \cr 0 & q & 1-q \end{bmatrix}\\] corresponding to eigenvalue \\(1\\)