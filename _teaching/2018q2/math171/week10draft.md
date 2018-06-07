---
layout: course_notes
number: Math 171
quarter: Spring 2018
week: 10
topics:
  - Poisson Process Conditioning
  - Renewal Process
hidden: True
---

1. **{{ page.topics[0] }}**

    1. Let \\(N(t)\\) be a Poisson process with rate \\(\lambda\\). Fix \\(0 \le n\\), \\(s \le t\\).
        1. Compute \\(\mathbb{P}(N(s)=m \mid N(t) = n)\\) for \\(m \le n\\). Give the name and parameters of the distribution.
        2. Compute \\(\mathbb{E}[N(s) \mid N(t) = n]\\)

    2. Let \\(N(t)\\) be a Poisson process with rate \\(\lambda\\) for \\(m \le k \le n\\). Fix \\(0 \le m \le n\\), \\(r \le s \le t\\).
        1. Compute \\(\mathbb{P}(N(s)=k \mid N(t) = n, N(r)=m)\\). Give the name and parameters of the distribution.
        2. Compute \\(\mathbb{E}[N(s) \mid N(t) = n, N(r)=m]\\)
        3. Compute the expected amount if time between the first and last arrivals in \\([r, t]\\) given that \\(N(t) = n\\) and \\(N(r)=m\\).

1. **{{ page.topics[1] }}**

    1. Cars queue at a gate. The lengths of the cars are i.i.d with distribution \\(F_L\\) and mean \\(\mu\\). Let \\(L \sim F_L\\). Each successive car stops leaving a gap, distributed according to a uniform distribution on \\((0, 1)\\), to the car in front (or to the gate in the case of the car at the head of the queue). Consider the number of cars \\(N(t)\\) lined up within distance t of the gate. Determine \\(\lim_{t \to \infty} \frac{\mathbb{E}[N(t)]}{t}\\) if 
        2. \\(L = c\\) is a fixed constant
        3. \\(L\\) is exponentially distributed with parameter \\(\lambda\\)
    2. Potential customers arrive at a service kiosk in a bank as a Poisson process of rate \\(\lambda\\). Being impatient, the customers leave immediately unless the assistant is free. Customers are served independently, with mean service time \\(\mu\\).
        1. Find the mean time between the starts of two successive service periods.
        2. Find the long run rate at which customers are served
        3. What proportion of customers who arrive at the bank actually get served?
