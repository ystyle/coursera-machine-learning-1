# Week 1 | II. Linear regression with one variable

## Question 1


Consider the problem of predicting how well a student does in her second year of college/university, given how well she did in her first year.

Specifically, let x be equal to the number of "A" grades (including A-. A and A+ grades) that a student receives in their first year of college (freshmen year). We would like to predict the value of y, which we define as the number of "A" grades they get in their second year (sophomore year).

Here each row is one training example. Recall that in linear regression, our hypothesis is hθ(x)=θ0+θ1x, and we use m to denote the number of training examples.



| x | y |
|---|---|
| 5	| 4 |
| 3	| 4 |
| 0	| 1 |
| 4	| 3 |

For the training set given above, what is the value of m? In the box below, please enter your answer (which should be a number between 0 and 10).

### Answer

m is the number of training examples. In this example, we have m=4 examples.

	4

---

## Question 2

Consider the following training set of m=4 training examples:

| x | y |
|---|---|
| 1	| 0.5 | |
| 2	| 1 |
| 4	| 2 |
| 0	| 0 |

Consider the linear regression model hθ(x)=θ0+θ1x. What are the values of θ0 and θ1 that you would expect to obtain upon running gradient descent on this model? (Linear regression will be able to fit this data perfectly.)

### Answer

- [ ] θ0=0.5,θ1=0

- [ ] θ0=1,θ1=0.5

- [ ] θ0=0.5,θ1=0.5

- [x] θ0=0,θ1=0.5

- [ ] θ0=1,θ1=1

---

## Question 3

Suppose we set θ0=0,θ1=1.5 in the linear regression hypothesis from Q1. What is hθ(2)?

### Answer

3

---

##Question 4

Let `f` be some function so that `f(θ0,θ1) `outputs a number. For this problem,`f` is some arbitrary/unknown smooth function (not necessarily thecost function of linear regression, so f may have local optima).Suppose we use gradient descent to try to minimize `f(θ0,θ1)` as a function of θ0 and θ1. Which of the following statements are true? (Check all that apply.)

### Answer

- [ ] No matter how θ0 and θ1 are initialized, so long as α is sufficiently small, we can safely expect gradient descent to converge to the same solution.

- [x] If the first few iterations of gradient descent cause f(θ0,θ1) to increase rather than decrease, then the most likely cause is that we have set the learning rate α to too large a value.

- [x] If θ0 and θ1 are initialized at the global minimum, then one iteration will not change their values.

- [ ] Setting the learning rate α to be very small is not harmful, and can only speed up the convergence of gradient descent.


---

## Question 5

Suppose that for some linear regression problem (say, predicting housing prices as in the lecture), we have some training set, and for our training set we managed to find some θ0, θ1 such that `J(θ0,θ1)=0`. Which of the statements below must then be true? (Check all that apply.)


### Answer

- [x] Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.

- [ ] Gradient descent is likely to get stuck at a local minimum and fail to find the global minimum.

- [ ] For this to be true, we must have y(i)=0 for every value of i=1,2,…,m.

- [ ] For this to be true, we must have θ0=0 and θ1=0 so that hθ(x)=0
