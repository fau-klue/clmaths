---
layout: default
title: Probability Theory
description: "A brief introduction into Probability Theory"
---

# Probability Theory

Probability plays an important role in computational linguistics. There are numerous models based on probability in different areas, such as Part-of-Speech tagging or probabilistic pragmatics. Probability distributions are also found in statistics.

## Introduction

Probabilities describe the likelihood of an outcome of a certain event. That means, the likelihood of the outcome 'heads' in a coin flip event is 50% (or 0.5). Every Probability lies somewhere between 0 and 1, with 0 meaning the outcome never occures and 1 meaning it always occures. Usually we see probability denoted with the letter $$p$$.

$$ 0 \leq p \leq 1 $$

In order to calculate the probability of an event, we can use a simple formula:

$$ Pr(Event) = \frac{Number\ of\ favorable\ outcomes}{Number\ of\ possible\ outcomes} $$

If we take the classic coin flip example, we would have the one favorable outcome $$heads$$ over the two possible outcomes $$heads$$ and $$tails$$.

$$ Pr(heads) = \frac{1}{2} = 0.5 $$

Now let's look at a more linguistical example. Let's say we want to guess a missing letter in a word. In this case, guessing a letter is the event:

$$ h\ \_\  t $$

There are several possible solutions (outcomes) of our, all of them might be correct (hat, hut, hit). We can describe all possible outcomes of an event as a set. This set is refered to as the sampple or probability space. In this case, it contains all letters in the english alphabet:

$$ S = \{a,b, \dots,z\} $$

Every letter has a certain likelihood of occuring between $$h$$ and $$t$$, even if that likelihood is 0. The sum of all likelihoods in our probability space adds up to 1, this is because one of the possible outcomes has to occure. If we take the coin flip example from before, the possible outcomes $$heads$$ and $$tails$$ both have a likelihood of 0.5, which also add  up to 1. Let formalize this, by using a function $$Pr$$, that will give us the probability (or likelihood) of an outcome.

$$ Pr(a) + Pr(b) + \dots + Pr(z) = 1 $$

$$ \sum\limits_{x \in S} Pr(x) = 1  $$

How can we find out the probability of a certain letter in the english alphabet? One possible solution would be to take a large amout of text and count how often each letter occures, then calculating the relative frequency (because all frequencies will add up to 1. Let's see a probability distribution of the all english letters:

<iframe width="100%" height="300" src="//jsfiddle.net/martialblog/c96prup7/1/embedded/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

## Joint Probability

$$ Pr(A,B) = Pr(A) \cap Pr(B) $$

## Conditional Probability

So far, we have looked at simple probabilities. Now let's us now see how we can adjust probabilities depending on conditions. We will continue with the example we have seen before, guessing a missing character in a word.

$$ h\ \_\  t $$

Here we have to guess the missing character between the h and the t. As we have seen before, taking the probability of the most likely character in the english language would lead us to choose e as the most favorable. However, we now want to factor in the information that we have already seen an h. The question we ask changes from "What is the most probable character?" to "What is the most probable character, given the previous character is an h?".

The general definition of conditional probability:

$$ Pr(A|B) = \frac{Pr(A) \cap Pr(B)}{Pr(B)} $$

This reads as: The probability of $$A$$ given $$B$$ is equal to, the joint probability of $$A$$ and $$B$$ divided by the probability of $$B$$.
