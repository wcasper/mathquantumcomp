---
layout: page
title: Complex numbers
---

## Imaginary numbers

Numbers come our intuitive ability to count things.  We can tell the difference between one apple or three and it is this difference between quantities that leads to the whole numbers.  Likewise addition exists intuitively: if we have three apples and five apples then together we have eight.  Likewise repeated addition leads to multiplication, and repeated multiplication leads to exponentiation.  All of these operations exist and are intuitively derived from the whole numbers.

Of course, we know the whole numbers are not the whole story.  So where do other numbers come from?  One answer is that they come from our desire to "undo" the operations that we have just described.  For example, undoing adding five apples leads to the idea of subtration.  Of course, when we subtract too many then we have a problem: too few apples to take away!  This leads to the construction of the negative numbers and thus to the **integers**.  In this way, we see that negative numbers are an invention created to allow usto make sense of expression of the form $$m-n$$, even when $$n>m$$.

Likewise, undoing multiplication leads to division. For example mutliplication by $$4$$ is ondone by division by $$4$$, so that while $$3\div 4=12$$ we have $$12/4= 3$$.
Here again, we realize that we have a problem for certain number combinations.  For example, $$5\div 4$$ doesn't make sense because $$5$$ is not a multiple of $$4$$. To fix this, we invent even more numbers, which we call the **rational numbers**.  Then we can write $$5\div 4 = 5/4$$.  Filling in numbers in between the various rational numbers (what mathematicians call *completing*) we end up with the **real numbers**.

From this point of view, it is only natural to consider what happens when we try to undo exponentiation.  For example, to undo the squaring operation $$3^2=9$$ we use the square root, getting $$\sqrt{9}=3$$.  Just like when we tried undoing addition and multiplication, we run into a problem: it doesn't yet make sense to undo squaring for negative numbers.  Our solution, just as it was in the previous two cases, is to create some more numbers where this operation makes sense!

**Definition:** The **imaginary number $$i$$** is a number satisfying $$i^2=-1$$.

We sometimes write this as $$i=\sqrt{-1}$$.  This makes it clear that $$i$$ is being introduced so as to allow us to undo squaring for negative numbers.  More generally, any number of the form $$ib$$ for some real number $$b$$ is called **imaginary**.  In particular $$ib$$ is a square root of $$-b^2$$.

The term *imaginary numbers* is regrettable, since it lends to a prejudice in our minds against imaginary numbers as "made up" or not part of the "real world".  Indeed, the name imaginary numbers was originally coined by Descartes, who named them so because he thought that they were ridiculous.  As we see above though, the invention of the imaginary numbers is just as legitimate as the invention of the negative integers or the rational numbers.  It comes from trying to make sense of undoing an operation we already know we can do for whole numbers.  Moreover, today we know that imaginary numbers play a profound and indispensable role in modern mathematics.  Indeed, if Descartes had known that even the great Hero of Alexandria had considered the notion of an imaginary number as far back as the first century, perhaps he wouldn't be so quick to judge!

In MATLAB, the imaginary number $$i$$ can be created using any of the following four commands

```Matlab
i
1i
j
1j
```

## Complex numbers

**Definition:** A **complex number** is any number $$z$$ of the form $$z=a + ib$$ where here $$a,b$$ are real numbers.

Examples of complex numbers include $$2 + 3i$$ and $$\sqrt{2} + (-1)i$$.  The need for complex numbers arises naturally from the desire to find roots of polynomial equations.  An equation like $$z^2+1=0$$ has no solutions over the real numbers, but two solutions over the complex numbers, namely $$z=\pm i$$.  In fact, over the complex numbers the Fundamental Theorem of Algebra is true.

**Fundamental Theorem of Algebra**:  Allowing for complex roots, any polynomal with $$p(z)$$ of degree $$n$$ has exactly $$n$$ has precisely $$n$$ roots, counting multiplicities.

### Properties of complex numbers

**Definition:** The **real part** $$\text{Re}(z)$$ of a complex number $$a+ib$$ is $$a$$.  The **imaginary part** $$\text{Im}(z)$$ of a complex number $$a+ib$$ is $$b$$.  The **modulus** or **absolute value** of $$z=a+ib$$ is

$$\lvert z\rvert = \sqrt{a^2 +b^2}.$$

**Definition:** The **complex conjugate** of $$z = a+ib$$ is $$\overline{z} = a-ib$$.

**Proposition:**  $$z\overline{z} = \lvert z\rvert^2$$


## Algebra with complex numbers

We can do all the usual operations with complex numbers
- addition:

$$(2 + 3i) + (5 + 7i) = 7 + 10i$$

- subtraction:

$$(2 + 3i) - (5 + 7i) = -2 - 4i$$

- multiplication

$$
\begin{align*}
(2 + 3i)\cdot (5 + 7i)
  & =  2\cdot 5 + 2\cdot 7i + 3i\cdot 5 + 3i\cdot 7i\\
  & =  10 + 14i + 15i + 21i^2\\
  & =  10 + 14i + 15i - 21\quad\text{(since $i^2=-1$)}\\
  & =  -11 + 29i
\end{align*}
$$

- division

$$
\begin{align*}
(2 + 3i) / (5 + 7i)
  & =  (2+3i)\cdot \frac{1}{5+7i}\\
  & =  (2+3i)\cdot \frac{1}{5+7i}\frac{5-7i}{5-7i}\\
  & =  (2+3i)\cdot \frac{5-7i}{(5+7i)(5-7i)}\\
  & =  (2+3i)\cdot \frac{5-7i}{74}\\
  & =  \frac{(2+3i)(5-7i)}{74}\\
  & =  \frac{31+i}{74}\\
  & =  \frac{31}{74} + \frac{1}{74}i
\end{align*}
$$




