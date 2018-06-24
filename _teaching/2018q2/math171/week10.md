---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 10
topics:
  - Poisson Process Conditioning
  - Renewal Process
  - Useful Formulas
---

1. **{{ page.topics[0] }}**

    1. Let \\(N(t)\\) be a Poisson process with rate \\(\lambda\\). Fix \\(0 \le n\\), \\(s \le t\\).

        1. Compute \\(\mathbb{P}(N(s)=m \mid N(t) = n)\\) for \\(m \le n\\). Give the name and parameters of the distribution.

            * (<font color="red">Answer</font>) Binomial(\\(n,\frac{s}{t}\\))

        2. Compute \\(\mathbb{E}[N(s) \mid N(t) = n]\\)

            * (<font color="red">Answer</font>) \\(n\frac{s}{t}\\)

    2. Let \\(N(t)\\) be a Poisson process with rate \\(\lambda\\). Fix \\(0 \le m \le n\\), \\(r \le s \le t\\).

        1. Compute \\(\mathbb{P}(N(s)-N(r)=k \mid N(t) = n, N(r)=m)\\). Give the name and parameters of the distribution.

            * (<font color="red">Answer</font>) Binomial(\\(n-m,\frac{s-r}{t-r}\\))

        2. Compute \\(\mathbb{E}[N(s) \mid N(t) = n, N(r)=m]\\)

            * (<font color="red">Answer</font>) \\((n-m)\frac{s-r}{t-r}\\)

        3. Compute the expected amount if time between the first and last arrivals in \\([r, t]\\) given that \\(N(t) = n\\) and \\(N(r)=m\\).

            * (<font color="blue">Solution</font>) For convenience of writing, I will omit the condition on \\(N(t) = n\\) and \\(N(r)=m\\) in the expectations.
            * Let \\(L\\) be the time of the last arrival in the interval, and \\(F\\) be the time of the first arrival in the interval. Then we seek \\[\begin{aligned}\mathbb{E}[L-F] &= \mathbb{E}[L] - \mathbb{E}[F]\\\\&=t - \mathbb{E}[t-L] - r - \mathbb{E}[F-r] \\\\&= (t-r) - \mathbb{E}[t-L] - \mathbb{E}[F-r].\end{aligned}\\] By symmetry, we can see that \\(t-L\\) (the time between the last arrival and the end of the interval) and \\(F-r\\) (the time between the start of the interval and the first arrival) have the same distribution, so \\[\mathbb{E}[L-F] = (t-r) - 2\mathbb{E}[F-r].\\]
            * Since we have conditioned on \\(N(t) = n\\) and \\(N(r)=m\\), we know that there are \\(n-m\\) arrivals uniformly distributed in the interval by the conditioning property of the poisson process. Therefore, letting \\(U\_1, \dots U\_{n-m}\\) be i.i.d uniform\\([0, t-r]\\) random variables, we have \\[\begin{aligned}\mathbb{E}[F-r] &= \mathbb{E}[\min(U\_1, \dots U\_{n-m})]\\\\&= \int\_0^{t-r}P(\min(U\_1, \dots U\_{n-m}) > s) ds\\\\&=\int\_0^{t-r}P(U\_1>s, \dots U\_{n-m}>s) ds\\\\&=\int\_0^{t-r}P(U\_1>s)^{n-m} ds\\\\&=\int\_0^{t-r}\left(\frac{t-r-s}{t-r}\right)^{n-m} ds\\\\&=-(t-r)\frac{\left(\frac{t-r-s}{t-r}\right)^{n-m+1}}{n-m+1} \Big\vert\_0^{t-r}\\\\&=\frac{t-r}{n-m+1}\end{aligned}\\]
            * So finally, we have \\[\begin{aligned}\mathbb{E}[L-F] &= (t-r) - 2\frac{t-r}{n-m+1}\\\\&=(t-r)\left(1-\frac{2}{n-m+1}\right)\end{aligned}\\]
            * As a sanity check, we check that if \\(n-m=1\\) we have \\(\mathbb{E}[L-F]=0\\), and if \\(n-m=\infty\\) we have \\(\mathbb{E}[L-F]=(t-r)\\)

1. **{{ page.topics[1] }}**

    1. Cars queue at a gate. The lengths of the cars are i.i.d with distribution \\(F_L\\) and mean \\(\mu\\). Let \\(L \sim F_L\\). Each successive car stops leaving a gap, distributed according to a uniform distribution on \\((0, 1)\\), to the car in front (or to the gate in the case of the car at the head of the queue). Consider the number of cars \\(N(t)\\) lined up within distance t of the gate. Determine \\(\lim_{t \to \infty} \frac{\mathbb{E}[N(t)]}{t}\\) if 

        2. \\(L = c\\) is a fixed constant

        3. \\(L\\) is exponentially distributed with parameter \\(\lambda\\)

    2. Potential customers arrive at a service kiosk in a bank as a Poisson process of rate \\(\lambda\\). Being impatient, the customers leave immediately unless the assistant is free. Customers are served independently, with mean service time \\(\mu\\).

        1. Find the mean time between the starts of two successive service periods.

            * (<font color="red">Answer</font>) \\(\mu + 1/\lambda\\)

        2. Find the long run rate at which customers are served

            * (<font color="red">Answer</font>) \\(\frac{1}{\mu + 1/\lambda}\\)

        3. What proportion of customers who arrive at the bank actually get served?

            * (<font color="red">Answer</font>) \\(\frac{1}{\lambda\mu + 1}\\)

    3. Customers arrive at a 24 hour restaurant (which has only one table) according to a poisson process with rate 1 party per hour. If the table is occupied, they leave immediately. If the table is unoccupied, they stay and eat. Customers spend an average of $20 each. The length of time a party stays is uniformly distributed in \\([0, N/2 \mathrm{\ hours}]\\) where \\(N\\) is the number of people in the party. Answer the following questions for the cases when \\(N\\) is uniform\\(\\{2, 3, 4\\}\\) and when \\(N\\) is geometric(\\(1/2\\)).

        1. Let \\(\tau\_k\\) be the time between when the \\((k-1)\\)st party finishes eating and the \\((k)\\)th party finishes eating. Compute \\(\mathbb{E}[\tau_k]\\)

            * (<font color="red">Answer</font>) \\(\mathbb{E}[N/4]+1\\)

        2. Let \\(X\_k\\) be the amount the \\((k)\\)th party spends. Compute \\(\mathbb{E}[X_k]\\).

            * (<font color="red">Answer</font>) \\(20\mathbb{E}[N]\\)

        3. Let \\(S(t)\\) the amount total amount paid by all parties by time \\(t\\). Compute \\(\lim\_{t\to \infty}\frac{S(t)}{t}\\), and justify the validity of your computation.

            * (<font color="red">Answer</font>) \\(\frac{20\mathbb{E}[N]}{\mathbb{E}[N/4]+1}\\). Justify by SLLN

1. **{{ page.topics[2] }}**

    1. For a discrete random variable \\(X\\) taking values in \\(\\{0, 1, 2, \dots\\}\\), we have \\(\mathbb{E}[X] = \sum\_{k=0}^\infty P(X > k)\\)

    1. For a continuous random variable \\(T\\) taking values in \\([0, \infty)\\), we have \\(\mathbb{E}[T] = \int\_0^\infty P(T > s) ds\\)

