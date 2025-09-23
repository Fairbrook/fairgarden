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
- $$ P(A \cup B) = P(A) + P(B) - P(A \cap B) $$

## 2.2 Counting Methods

### Fundamental Principle of Counting

$$ k $$ operations are to be performed. If there are $$ n_1 $$ ways to perform the first operation, and if for each 
of these ways there are $$ n_2 $$ ways to perform the second operation, and if for each choice of ways to perform the first two operations there are $$ n_3 $$ ways to perform the third operation, the total number of ways to perform the sequence of $$ k $$ operations is $$ n_1n_2 \cdots n_k $$

### Permutations

Ordering of a collection of objects. 

The number of permutations of n objects is 
$$
n!
$$
The number of permutations of k objects chosen from a group of n objecs is
$$
\frac{n!}{(n-k)!}
$$


### Combinations

Choosing groups of objects that can be selected without regard to order
$$
\begin{pmatrix}
n\\
k
\end{pmatrix}
=
\frac{n!}{k!(n-k)!}
$$

The number of ways of dividing a group of n objects into groups of $$ k_1,\cdots,k_r$$ where $$ k_1 + \cdots + k_r = n $$ is

$$
\frac{n!}{k_1! \cdots k_r!}
$$


## 2.3 Conditional Probability and Independence


### Unconditional probability

A probability based on the entire sample space


### Conditional probability

A probability that is based on a part of a sample space

Let $$A$$ and $$B$$ be events with $$P(B)\neq0$$. The conditional probability of $$A$$ given $$B$$ is
$$
P(A|B) = \frac{P(A \cap B)}{P(B)}
$$

### Independent Events

The knowledge that one event has occurred does not change the probability that another event occurs

Two events are independent if the probability of each event remains the same whether or not the other occurs

$$
\text{If } P(A) \neq 0 \text{ and } P(B) \neq 0 \text{ then } A \text{ and } B \text{ are independent if } \\
P(B|A) = P(B) \\
P(A|B) = P(A)
$$

### The Multiplication rule

$$
 P(A \cap B) = P(B)P(A|B)\\
 P(A \cap B) = P(A)P(B|A)
$$

When two events are independent then the multiplication rules simplifies

$$
P(A \cap B) = P(A)P(B)
$$

### The law of total probability

If $$A_1, \cdots , A_n$$ are mutually exclusive and exhaustive events, and $$ B $$ is any event, then

$$
P(B) = P(A_1 \cap B) + \cdots + P(A_n \caps B)
$$

Equivalently

$$
P(B) = P(B|A_1)P(A_1) + \cdots + P(B|A_1)P(A_1)
$$


### Bayes' Rule

Rule to calculate the conditional probabilities of $$ P(B|A) $$ knowing $$ P(A|B) $$
$$
P(A|B) = \frac{P(B|A)P(A)}{P(B)} = \frac{P(B|A)P(A)}{P(B|A)P(A)+P(B|A^C)P(A^C)}
$$


## 2.4 Random Variables

Assings a numerical value to each outcome in a sample space


### Discrete variables

The possible values are arranged in order, there is a gap between each value and the next one


#### Probability mass function

The probability mass function of a discrete random variable X is the function $$p(x) = P(X=x)$$. 
Also called the probability distribution

#### Cumulative distribution function

Specifies the probability that a random variable is less than or equal to a given value
$$
F(x) = P(X \leq x)  = \sum_{t \leq x}{p(t)} = \sum_{t \leq x}{P(X=t)}
$$
$$
\sum_{x}{p(x)} = \sum_{x}{p(x)} = 1
$$

#### Mean

Let $$X$$ be a discrete random variable with probability mass function $$p(x)=P(X=x)$$

The mean of $$X$$ is given by 
$$
\mu_x = \sum_{x}xP(X = x)
$$
Also called expectation, expected value or $$E(X)$$


#### Standard deviation

Let $$X$$ be a discrete random variable with probability mass function $$p(x)=P(X=x)$$

- The variance of X is given by
$$
\+sigma_X^2 = \sum_{x}{(x-\mu)^2P(X=x)}
$$

- An alternative formula for the variance is given by

$$
\+sigma_X^2 = \sum_{x}{x^2P(X=x)-\mu_X^2}
$$

- The standard deviation is the square root of the variance 

$$
\sigma_X = \sqrt{\sigma_X^2}
$$


#### The Probability Histogram

![Histogram](./data-science/imgs/probability-histogram.png)

