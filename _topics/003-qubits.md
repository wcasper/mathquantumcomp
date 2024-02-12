---
layout: page
title: Qubits
---

Quantum bits or **qubits** are the fundamental building blocks of quantum computers.
They are analogous to classical bits in a computer -- the zeros and ones which are used to store basic information.
However, unlike with classical bits, as single qubit contains much more information than a simple $$0$$ or a $$1$$.
In particular, it can be thought of as existing in a state of uncertainty, with a certain probability of being one or the other $$0$$.

The real good stuff happens when we put more than one qubit together.
Then qubits can exhibit quantum behaviors like **entanglement**, where the state of one qubit influences the state of another, even when they aren't very close together.
This leads to amazing theoretical algorithms, like **Schor's algorithm** which have the potential to revolutionize our technological landscape.

When we actually try to make a qubit, we need to create some kind of quantum system with two main possible states (or energy levels), corresponding to being a $$0$$ or a $$1$$.
Physicists and engineers use all kinds of interesting tactics for this, including:
* superconducting circuits and Josephson junctions,
* trapping ions in magnetic fields,
* using polarized states of photons,

and many more.
However, these topics have to do with the hardware of a quantum computer.
Our goal is to understand the *mathematics* that will be needed to understand current quantum algorithms and create new algorithms, on whatever sort of quantum computers are built in the future.

## What is a Qubit
We need a mathematical object which describes something which is simultaneously a $$0$$ with a certain probability and a $$1$$ with another certain probability.
Mathematically, this is easy to accomplish.

**Definition:** A **qubit** is a vector $$\binom{a}{b}$$, where here $$a$$ and $$b$$ are complex numbers with the property that it is **normalized**, meaning $$\lvert a\rvert^2 + \lvert b\rvert^2 = 1$$.

Put another way, we can think about qubits as unit vectors in a two-dimensional vector space, but where our scalars are complex numbers.

The normalization here is *essential*.
The value of $$\lvert a\rvert^2$$ is the probability that when we observe it the qubit will say $$0$$.
Likewise, the value of $$\lvert b\rvert^2$$ is the probability that our observation gives us a $$1$$.
Put together, these probabilities should add up to $$1$$.

What we mean by observing is worth visiting in more detail.
Our intuition comes from the story of Schr\"{o}diger's cat.
The physicist Erwin Schrödinger imagines (and only imagines, to avoid legal trouble) putting his cat inside a box along with a radioactive atom, a Geiger counter, a vial of poison, and a hammer. If the atom decays, the Geiger counter will observe it and trigger the hammer to smash the vial and kill the cat.
However, until we open the box we won't see whether the cat is dead or not.
This is where quantum stuff gets weird.
According to quantum mechanics (or at least one interpretation of it) the cat is simultaneously both alive and dead with certain probabilities.
When we **observe** the state of the system, the probability instantly changes and the cat is either all alive or all dead.



**Question:** Is $$\binom{2}{\sqrt{3}i}$$ a qubit?
<details>
  <summary>Click for answer.</summary>
  No, because it isn't normalized.
</details>

### Notation
Vectors themselves are so important there are usually many different notations used to describe them.
This kind of thing tends to happen with important topics, since many different disciplines have convenient ways of describing things for their subject.
In Calculus III, we often use $$\textbf{i},\textbf{j},\textbf{k}$$-notation to describe vectors, so that $$a\textbf{i} + b\textbf{j} + c\textbf{k}$$ represents a vector pointing from the origin to the point $$(a,b,c)$$.

In quantum mechanics, we have a different notation coming from physics, called **bra** and **ket** notation (put together, it sounds like "bracket").
In place of $$\mathbf{i}$$ and $$\mathbf{j}$$, we use the symbols $$\ket{0}$$ and $$\ket{1}$$.
So for us

$$a\ket{0} + b\ket{1}$$

means the same thing as $$\binom{a}{b}$$.






