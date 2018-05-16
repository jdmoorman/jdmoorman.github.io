---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 7
topics:
  - Martingales
  - Optional Stopping
hidden: True
---

1. **{{ page.topics[0] }}**

    2. Let \\((X\_n)\_{n \ge 0}\\) be i.i.d. uniform on \\([-1, 0) \cup (0, 1]\\)

        3. Show that \\((M\_n)\_{n \ge 0}\\) with \\(M\_n = X\_0 + \dots + X\_n\\) is a Martingale.

        3. Show that \\((M\_n)\_{n \ge 0}\\) with \\(M\_n = \frac{1}{X\_0} + \dots + \frac{1}{X\_n}\\) is not a Martingale.

    2. Let \\((X\_n)\_{n \ge 0}\\) be i.i.d. uniform on \\(\\{-1, 1\\}\\). AKA Rademacher distributed. Let \\(S\_n = X\_0 + X\_1 + \dots + X\_n\\) for some \\(X\_0\\).

        3. Compute the moment generating function of \\(S\_n\\). That is, \\(\mathbb{E}[e^{tS\_n}]\\)

        3. Find the odd moments of \\(S\_n\\). That is, \\(\mathbb{E}[S\_n^{2m+1}]\\). Explain briefly why the result makes sense.

        3. Find the even moments of \\(S\_n\\). That is, \\(\mathbb{E}[S\_n^{2m}]\\).

        3. For what value of \\(c\\) is \\(M\_n = S\_n^2 - nc\\) a martingale?

        3. Find a formula for \\(\mathbb{E}[S\_{n+1}^{2m} \mid S\_n=t]\\) which depends only on \\(m\\) and \\(t\\)

1. **{{ page.topics[1] }}**

    2. Textbook (3rd edition) problems 5.8, 5.9

    2. Textbook (3rd edition) problems 5.16, 5.17