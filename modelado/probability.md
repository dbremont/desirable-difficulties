# Probability

- You have three children, but only one apple. You want to toss a fair coin to determine which child gets the apple. You want each child to be equally likely to get the apple. What is your strategy?
- You are blindfolded and faced with 100 coins on a table, 10 of which show heads and 90 show tails. Without being able to see the coins, how can you divide them into two groups such that each group has the same number of heads?
- **Amoeba population**: There is one amoeba in a pond. After every minute the amoeba may die, stay the same, split into two, or split into three with equal probability. All its offspring, if it has any, will behave the same (and independent of other amoebas).  **What is the probability the amoeba population will die out?**
- A certain disease affects 1% of the population. A diagnostic test for the disease has a **99% sensitivity** (i.e., it correctly identifies 99% of people who have the disease) and a **95% specificity** (i.e., it correctly identifies 95% of people who do not have the disease).

     A randomly selected person from the population takes the test and receives a **positive** result.

     **What is the probability that the person actually has the disease?**

- Suppose that for three fair dice. Denote the scores obtained by X1, X2 and X3. Find P(X1 +X2 +X3 ≤5).
- Two real numbers X and Y are chosen at random in the interval (0, 1).
Compute the probability that the closest integer to X/Y is even.
- `If every family has a child until a boy is born; what will the average proportion of boys to girls be?`

---

For each of the following scenarios, find the requested probability. Assume the sets $A, B,$ and $C$ are events from the same sample space $S$. (Hint: Venn diagrams may help with the visualization, although they are not required to answer the questions.)

If $P(A) = .4, P(B^c) = .7,$ and $P(A \cap B^c) = .2,$ find $P(A \cap B)$

---

For each of the following scenarios, find the requested probability. Assume the sets $A, B,$ and $C$ are events from the same sample space $S$. (Hint: Venn diagrams may help with the visualization, although they are not required to answer the questions.)

If $P(A) = 0.9$ and $P(B) = 0.9$, what is the lower bound for $P(A \cup B)$.

---

Three popular options on a certain type of car are $A$ leather seats, $B$ a sunroof, and $C$ heated seats. In the past, $P(A) = 0.55$ (i.e. 55% of the customers have requested option $A$), $P(B) = 0.45, P(C) = 0.4$. Furthermore, $P(A \cap B) = 0.25, P(A \cap C) = 0.2, P(B \cap C) = 0.15$ and $P(A \cap B \cap C) = 0.1$.

Find the probability that a customer will ask for at least one of the three options.

---

Three popular options on a certain type of car are $A$ leather seats, $B$ a sunroof, and $C$ heated seats. In the past, $P(A) = 0.55$ (i.e. 55% of the customers have requested option $A$), $P(B) = 0.45, P(C) = 0.4$. Furthermore, $P(A \cap B) = 0.25, P(A \cap C) = 0.2, P(B \cap C) = 0.15$ and $P(A \cap B \cap C) = 0.1$.

Find the probability that a customer will not ask for any of these three options.

---

Three popular options on a certain type of car are $A$ leather seats, $B$ a sunroof, and $C$ heated seats. In the past, $P(A) = 0.55$ (i.e. 55% of the customers have requested option $A$), $P(B) = 0.45, P(C) = 0.4$. Furthermore, $P(A \cap B) = 0.25, P(A \cap C) = 0.2, P(B \cap C) = 0.15$ and $P(A \cap B \cap C) = 0.1$.

Find the probability that a customer will ask for heated leather seats but not a sunroof.

---

Three popular options on a certain type of car are $A$ leather seats, $B$ a sunroof, and $C$ heated seats. In the past, $P(A) = 0.55$ (i.e. 55% of the customers have requested option $A$), $P(B) = 0.45, P(C) = 0.4$. Furthermore, $P(A \cap B) = 0.25, P(A \cap C) = 0.2, P(B \cap C) = 0.15$ and $P(A \cap B \cap C) = 0.1$.

Find the probability that a customer will ask for at most two of the options.

---

Three popular options on a certain type of car are $A$ leather seats, $B$ a sunroof, and $C$ heated seats. In the past, $P(A) = 0.55$ (i.e. 55% of the customers have requested option $A$), $P(B) = 0.45, P(C) = 0.4$. Furthermore, $P(A \cap B) = 0.25, P(A \cap C) = 0.2, P(B \cap C) = 0.15$ and $P(A \cap B \cap C) = 0.1$.

Find the probability that a customer will ask for exactly two of the options.

---

A message of length 5 digits is to be sent. Each digit can be a 0, 1, or 2.

What is the cardinality of the sample space?

---

A message of length 5 digits is to be sent. Each digit can be a 0, 1, or 2.

If every message is equally likely, what is the probability that the message consists of 2 zeros, 2 ones, and 1 two? Round your answer to have four decimal places.

---

A message of length 5 digits is to be sent. Each digit can be a 0, 1, or 2.

What is the probability that the message contains at least one zero? Round your answer to have three decimal places.

--

```R
#Imports test that library
library(testthat)
```

### Problem 1:
Suppose we are interested in the buying habits of shoppers at a particular grocery store with regards to whether they purchase apples, milk, and/or bread. Now suppose 30\% of all shoppers at this particular grocery store buy apples, 45\% buy milk, and 40\% buy a loaf of bread. Let $A$ be the event that a randomly selected shopper buys apples, $B$ be the event that the same randomly selected shopper buys milk, and $C$ the event that they buy bread.  Suppose we also know (from data collected) the following information:


*   The probability that the shopper buys apples and milk is 0.20.
*   The probability that the shopper buys milk and bread is 0.25.
*   The probability that the shopper buys apples and bread is 0.12.
*   The probability that the shopper buys all three items is 0.07.

Use this information to answer the following questions.

**a)** For our purposes, we will use a numeric representation for each event. For example, $(010)$ would be an event in the sample space where a zero in the first place represents no apples were bought while a 1 means they were. Similarly,  the second place is the presence of milk and the third place of bread. The example given $(010)$ represents the purchase of milk but not apples or bread.

Insert into vector `S` the events that belong to the sample space. Then insert the events from the sample space that would correspond to $A$ occuring into vector `A`. Repeat this with vector `B` for $B$ and vector `C` for $C$.

According to set notation, the sample space should look like this: $S=\{ \dots \}$. However, due to data storage syntax in R, we will be storing these events in vectors. For example, for some arbitrary event $W$ would be stored as follows $W=c(010)$. `c()` is a command we can use to construct a vector where commas separate each entry. Complete the code below. Do not worry about the order in which events are placed in vector.


```R
S = c(000, 001, 010, 011, 100, 101,  110, 111)
A = c(100, 101, 110, 111)
B = c(010, 011, 110, 111)
C = c(001, 011, 101, 111)

```


```R
# Test cell
```


```R
# Hidden test cell
```


```R
# Hidden test cell
```


```R
# Hidden test cell
```

**b)** Find the probability that the shopper purchases at least one of the three items.

Store your answer in a variable `p1.1`.


```R
p1.1 = 0.30 + 0.45 + 0.40 - 0.20 - 0.12 - 0.25 + 0.07

```


```R
# Hidden test cell
```

**c)** Find the probability that the shopper purchases none of the three items.

Store your answer in a variable `p1.2`.


```R
p1.2 = 1 - p1.1

```


```R
# Hidden test cell
```

**d)** Find the probability that the shopper buys milk and bread but not apples.

Store your answer in a variable `p1.3`.


```R
p1.3 = 0.25 - 0.07

```


```R
# Hidden test cell
```

### Problem 2:

A student takes a multiple choice test with $20$ questions. Each question has 5 possible answers, only one of which is correct.

**a)** How many ways can the test be completed?  (Find the cardinality of the sample space.) Store your answer in `cardinality`.


```R
cardinality = 5**20
cardinality

```


95367431640625



```R
# Hidden test cell
```

**b)** If a student answers each question at random, what is the probability that they will answer at least $14$ questions correctly? Round your answer to seven decimal places. Store your answer in `p2.b`.


```R
p2.b = sum(dbinom(14:20, size=20, prob=0.2))
```


```R
# Hidden test cell
```

**c)** If a student knows the answer to each question with probability $0.9$, what is the chance they will answer at least $14$ correctly? Round your answer to four decimal places. Save your answer as `p2.c`.


```R
p2.c = sum(dbinom(14:20, size=20, prob=0.9))

```


0.997613910591034



```R
# Hidden test cell
```

Thought question (Ungraded): If a student understands 90\% of the material, is a multiple choice test of 20 questions an appropriate means of testing?

### Problem 3:

Suppose there are 20 employees on the day shift, 15 on swing, and 10 on nights. You would like to choose 6 at random for an in-depth interview. Let $A_{1}$ be the event that all 6 are chosen from the day shift, $A_{2}$ be the event that all $6$ are chosen from the swing shift, and $A_{3}$ the event that all 6 are chosen from the night shift.

**a)** What is the cardinality of the sample space (the drawing of 6 employees from all shifts)? Assume each employee is unique. Think about what each element, or possible outcome, in the sample space represents.


```R
total_employees = 20 + 15 + 10
Size = choose(total_employees, 6)
Size
```


8145060



```R
# Hidden test cell
```

**b)** Assuming that each employee is chosen with equal probaiblity, what is the probability that all 6 chosen employees work the day shift? Note that the employees are chosen sequentially, not all at once. Round your answer to 5 decimal places. Save your answer as `P_AllDay`. 

Thought question (ungraded): If you hired a consultant to do this interview and all 6 employees were chosen from the day shift, what would you be likely to conclude?


```R
P_AllDay = choose(20, 6) / Size
P_AllDay

```


0.00475871264300079



```R
# Hidden test cell
```

**c)** What is the probability that all 6 workers are selected from the same shift? Again, assume the employees are selected sequentially and not all at once. Round your answer to four decimal places. Save your answer as `P_AllSame`.


```R
P_AllSame = choose(20, 6) / Size + choose(15, 6) / Size +  choose(10, 6) / Size
print(P_AllSame)

```

    [1] 0.005398978



```R
# Hidden test cell
```

Thought question (Ungraded): Let $B_{1}$ be the event that no one from the day shift is selected, $B_{2}$ the event that no one from the swing shift is selected, and $B_{3}$ the event that no one from the night shift is selected. 

How is $A_{1}^{c}$ defined? Is it related to $B_{1}$ or $B_{1}^{c}$? It's very important to carefully define the events of interest so that you know you are calculating the correct probability.

**d)** Find the probability that at least one of the shifts will be unrepresented in the sample of $6$ workers. Round your answer to four decimal places. Save your answer as `P_NoneOfOneShift`.

**Hint:** We want to solve $P(B_1 \cup B_2 \cup B_3)$. To solve this, it may help to make a venn diagram for these events. Make sure you don't overcount the overlapping areas of this venn diagram!


```R
P_NoneOfOneShift = 1 - (choose(19 + 14 + 9, 3) / Size)
print(P_NoneOfOneShift)

```

    [1] 0.9985906



```R
# Hidden test cell
```
