---
title: Chapter 2 - Probability
---

## 2.1 Basic Ideas

### Experiment

Process that results in an outcome that cannot be predicted in advance with certainty. For example:

- Tossing a coin
- Rolling a die
- Weighing the contents of a box of cereal
- Measuring the diameter of a bolt

### Sample space

The set of all possible outcomes of an experiment

### Event

A subset of a sample space

### Combining Events

Notations to combine multiple events 

#### Union

Set of outcomes that belong to either A, to B, or to both. __A or B or Both__

![Union](./data-science/imgs/union.png)

#### Intersection

Set of outcomes that belong to both A and B. __Both A and B__

![Intersection](./data-science/imgs/intersection.png)

#### Complement

Set of outcomes that do not belong to A. __A does not occur__

![Complement](./data-science/imgs/complement.png)


### Mutually exclusive Events

A collection of events A, B, C,...,Z is said to be mutually exclusive if no two of them have any outcomes in common

### Probabilities

Given any experiment and any event A:

- The expression P(A) denotes the probability that the event A occurs
- P(A) is the proportion of times that event A would occur in the long run, if the experiment were to be repeated

#### Axioms of probability

- Let S be a sample space. Then P(S) = 1
- For any event A,  0 <= P(A) <= 1
- If A and B are mutually exclusive events, then P(AUB) = P(A) * P(B)
- $$ P(A^c) = 1 - P(A) $$
- $$ P(\emptyset) = 0 $$
- $$ P(A) = \frac{k}{N} $$
- $$ P(A \union B) = P(A) + P(B) - P(A \intersection B) $$

