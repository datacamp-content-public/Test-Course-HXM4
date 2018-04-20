---
title: Test Chapter 1
description: This is a template chapter.
---

## Exercise 1

```yaml
type: MultipleChoiceExercise
lang: r
xp: 50
skills: 1
key: a20fcf7b57
```

Suppose you poll a population in which a proportion $p$ of voters are Democrats and $1-p$ are Republicans. Your sample size is $N = 25$. Consider the random variable $S$, which is the **total** number of Democrats in your sample. 

What is the expected value of this random variable $S$?

`@instructions`
- $$\mbox{E}(S) = 25(1-p)$$
- $$\mbox{E}(S) = 25p$$
- $$\mbox{E}(S) = \sqrt{25 p (1-p)}$$
- $$\mbox{E}(S) = p$$

`@hint`
- $$\mbox{E}(S)$$ is a function of a function of $p$ and the sample size.

`@sct`
```{r}
msg1 = "Try again. This selection tells you the expected value of a random variable for the number of Republicans in your sample."
msg2 = "Nice work!"
msg3 = "Try again. The expected value of `S` is related to the sample size and the proportion of Democrats in your sample."
msg4 = "Try again. You also need to consider the sample size."
test_mc(correct = 3, feedback_msgs = c(msg1,msg2,msg3,msg4))
```


---
## Exercise 2

```yaml
type: MultipleChoiceExercise
key: 2e9781fee1
lang: r
xp: 50
skills: 1
```

Again, consider the random variable $S$, which is the **total** number of Democrats in your sample of 25 voters. The variable $p$ describes the proportion of Democrats in the sample, whereas $1-p$ describes the proportion of Republicans.

What is the standard error of $S$?

`@instructions`
- $$\mbox{SE}(S) = 25 p (1-p)$$
- $$\mbox{SE}(S) = \sqrt{25p}$$
- $$\mbox{SE}(S) = 25(1-p)$$
- $$\mbox{SE}(S) = \sqrt{25 p (1-p)}$$

`@hint`
- The standard error is a function of `p` and the sample size.

`@sct`
```{r}
msg1 = "Try again. The units of variance are squared."
msg2 = "Try  again. The standard error is affected by the proportions of both Republicans and Democrats."
msg3 = "Try again. The standard error is affected by the proportions of Democrats and Republicans."
msg4 = "Nice work!"
test_mc(correct = 4, feedback_msgs = c(msg1,msg2,msg3,msg4))
```