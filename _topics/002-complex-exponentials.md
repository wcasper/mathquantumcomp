---
layout: page
title: Complex exponentials
---
##  Euler's Formula

**Euler's Formula** is

$$e^{i\theta} = \cos(\theta) + i\sin(\theta)$$

As a special case, we have the beautiful identity featuring all the special numbers we know

$$e^{i\pi} + 1 = 0.$$

Using this, we can write any complex number in the form

$$z=re^{i\theta} = r\cos(\theta) + ir\sin(\theta)$$

for some $$r\geq0$$ and $$0\leq \theta<2\pi.$$

The value $$r$$ here corresponds to the modulus of $$z$$ and $$\theta$$ corresponds to the angle of the associated vector counter-clockwise from the $$x$$-axis.


### Proving trig identities with Euler's formula

Consider the product of complex numbers

$$(\cos\theta + i\sin\theta)(\cos\phi + i\sin\phi) = \cos\theta\cos\phi-\sin\theta\sin\phi + i(\cos\theta\sin\phi + \sin\theta\cos\phi)$$

We can use Euler's formula to calculate this a different way

$$(\cos\theta + i\sin\theta)(\cos\phi + i\sin\phi) = e^{i\theta}e^{i\phi} = e^{i(\theta+\phi)} = \cos(\theta+\phi) + i\sin(\theta + \phi)$$

This leads to the **angle addition formulas** for sine and cosine

$$\cos(\theta + \phi) = \cos\theta\cos\phi-\sin\theta\sin\phi$$

$$\sin(\theta + \phi) = \sin\theta\cos\phi+\cos\theta\sin\phi$$


## De Moivre's Formula
As a special case of Euler's formula, we have De Moivre's formula linking complex numbers with trigonometry.

$$(\cos(\theta) + i\sin(\theta))^n = \cos(n\theta) + i\sin(n\theta).$$

## Roots

The $$n$$'th root of  a complex number is 

$$\left(re^{i\pi}\right)^{1/n} = r^{1/n}e^{i\pi/n}.$$

$$z = re^{i\theta}$$

## Special cases

**Example:** 
We can write

$$i^i = (e^{i\pi/2})^i =  e^{i^2\pi/2} = e^{-\pi/2}$$

**Example:**

What is the value of $$(1 + i)^{2021}$$ ? 


## Roots of unity

An **n'th root of unity** is a complex number  $$z$$ satisfying $$z^n=1$$.  From the degree, we expect this equation to have $$n$$ solutions, ie. $$n$$ roots of unity.  These are given by

$$z = e^{2\pi ik/n} = \cos(2\pi k/n) + i\sin(2\pi k/n),\quad k=0,1,\dots, n-1$$

## Additional resources



