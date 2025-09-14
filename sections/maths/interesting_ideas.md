---
layout: default
title: To investigate
section_order: 0
section_key: maths
date: 2025-09-03
permalink: /mathematics/interesting-ideas
---

# Concepts to play around with

Here are mathematical and algorithmical concepts that I find interesting and would like to spend some time thinking about them.

## Divisibility rule for 11

This rule is very useful for checksums. For example Czech birth numbers and banking numbers use this divisibility rule. The rule is as follows  sum up all digits on odd positions and subtract all digits on even position. If the resulting number is divisible by 11, then the original number is divisible by 11.

The goal would be to figure out how the rule works and prove it mathematically.

## Understand RSA key generation

I already know the general concept that makes RSA work.

They keys are exponents $e,d$, the message is a number $x$ and codeword is $c = x^e$. We want to achieve decryption using $c^d = x^{ed}$.

We are counting modulo some big number $n = p \cdot q$ where $p,q$ are big prime numbers. Because of this fact, we know the *Euler function* of $n$ but nobody else cannot simply compute the result without factoring $n$ even if they know $n$. In particular we have $\varphi(n) = pq - p - q + 1$. 

Then we use *Euler's formula* which states that for any $x$ s.t. $\gcd(n,x) = 1$ we have $x^{\varphi(n)} = 1$. So we want that $ed \equiv 1 \pmod{\varphi(n)}$. For this we use the *Bezout's formula* which states that for any $x,y$ there exist $u,v$ s.t. $\gcd(x,y) = x \cdot u + y \cdot v$ (see *Extended Euclid's algorithm*).

Now since we have $\gcd(d,\varphi(n)) = 1$, we have $1 = d \cdot e + \varphi(n) \cdot k$ for some number $k$. By this fact, we see that $x^{ed} \equiv x^{1 - \varphi(n) \cdot k} \equiv x$.

The goal here would be to see how this is done in practice. How the numbers are chosen and whether we can see what numbers were chosen if we investigate the program.

## Come up with visualisations of

Motivation for this is, that the logarithmic rules we learned at high school were always hard for me to remember. I could derive it but it took me too long and the derivation was very symbolical, lacking intuition. I was wondering whether I could find some visualisation of this rule which would also serve as a good mnemotechnic to remember it for the rest of my lifetime.

### Logarithm rules

Consider the formula $\log_a{b} \cdot log_b{c} = log_a{c}$. 

Note that it is quite useful formula since it shows us that the ratio between $log_b{c}$ and $log_a{c}$ is just $log_a{b}$ which for fixed $a,b$ is constant. So changing the base of a logarithm will not influence asymptotics when analyzing speed of algorithms.

What would be the visualisation? The right side asks, how many times we can fit $a$ into $c$ by writing it as $c = \overbrace{a \cdot a \cdot \ldots \cdot a}^{log_a{c}}$. The problem is, that we only know $b = \overbrace{a \cdot a \cdot \ldots \cdot a}^{log_a{b}}$ and $c = \overbrace{b \cdot b \cdot \ldots \cdot b}^{log_b{c}}$.

But this is nice now ce can just plug in for each $b$ in the last equation the amount of $a$'s corresponding to $\log_a{b}$. So we have $c = \overbrace{b \cdot \underbrace{b}_{a \cdot a \cdot \ldots \cdot a} \cdot \ldots \cdot b}^{log_b{c}}$. 

So now how many $a$'s are there in $c$? 

Well in every $b$ there is $log_a{b}$ of them and there is $log_b{c} \space$ $b$'s in $c$ so in total we have $log_a{b} \cdot log_b{c} \space $ $a$'s in $c$.

## Find where certain types of functions naturally appear in life

Goal of this topic is to categorize types of functions and find real life examples for each category. This collection should then serve teachers as a repository of answers when students ask: Why do we learn about these functions?

### Linear functions

How we age is linear. Consider the following problem: I am 24 years old and my father is 60 years old. In how many years will my father be exactly twice as old as me?

The question stated mathematically is find $x$ s.t. $2 \cdot (24 + x) = 60 + x$.

### Quadratic functions

TODO:

## Where are math concepts useful

Again, this chapter serves a motivational purpose. Now we just don't restrict ourselves to types of analytic functions but consider all mathematical concepts in general.

### Prime numbers
- cryptography.