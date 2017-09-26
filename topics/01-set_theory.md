---
layout: default
title: Set Theory
description: "A brief introduction into Set Theory"
---

# Set Theory

This course will teach you some elementary Set Theory. We look at basic properties of sets, how to define a set, and how to compare different sizes of sets.

## Introduction

Sets can be found almost anywhere. For example, we can define a set of all humans on the planet and take one person as an element of that set. All the words in a language can be seen as a set, a word as an element of it. Now for some formal definitions.

To define a set $$A$$ with the elements $$1,2,3$$ we write:

$$ A = \{1,2,3\} $$

If we have an element $$a$$, that is in our set, we write:

$$ a \in A $$

If we have an element $$b$$, that is not in our set, we write:

$$ b \notin A $$

Now we can easily describe the state of our world like so:

$$ B = \{I, you, he, she, it, we, they\} $$

$$ you \in B $$

$$ his \notin B $$

Sets are defined by their elements, not by the order of their elements. That means $$\{1,2,3\} $$ and $$\{3,1,2\} $$ is the same set. Also, sets know only unique elements. The set $$\{1,2,3\} $$ and $$\{1,1,2,2,3,3\}$$ is still the same set. We don't always have to, or can, write down all elements in a certain set. In this case, we will use a shorthand notation $$\{a,b,c,\dots\}$$.

We can visualize sets using Venn Diagrams. Here we define two different sets, that have no elements in common. Venn Diagrams will come in handy later, when we see different set operations.

<iframe width="100%" height="300" src="//jsfiddle.net/martialblog/1mkjpxsv/embedded/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

Enumerating all elements is possible for small sets, however if we have many (or infinite) elements in one set, we rather describe elements by their properties. For a property $$P$$ and an element $$e$$ of a set $$S$$, we write $$P(e)$$ to indicate that $$s$$ has the property $$P$$. Now we have the possibility to shorten our notation:

$$ A = \{e ∈ S : P(e)\} $$

This reads: The set $$A$$ consists of all elements $$e$$, of the set $$S$$, with the property $$P$$. The colon $$:$$ is read a "such as".

Finally, we have to define a special set: The Set that contains no elements. Any set without elements is called an "Empty Set" and is notated as such:

$$ Z = \{\} $$

$$ Z = \emptyset $$

## Subsets

When talking about sets, we often need to describe subsets. Subsets $$\subset$$ contain some, or all, elements of another set. A proper subset $$\subseteq$$ contains only some elements of another set.

Let's first define some simple sets:

$$ A = \{1,2,3\} $$

$$ B = \{0,2,4\} $$

$$ C = \{4\} $$

We can notate subsets like this:

$$ C \subset B $$

$$ \{1,2,3\} \subseteq A $$

Here we see that $$C$$ is a proper subset of $$B$$, since it contains some of the elements of $$B$$ but not all of them. We also see that the set $$ \{1,2,3\} $$ is a subset of $$A$$, since it contains all the elements of it.

We can also notate the opposite, when the subset property is not given. For example, $$A$$ is not a subset of $$B$$:

$$ A \not\subset B $$

## Operations

### Union

To extend our capabilities to work with sets, we can also define some operations. These are similar to arithmetic operations like addition or subtraction.

First, let's look at Unions. Unions allow us to combine two or more sets to extend them. Here is an example using the sets we previously defined:

$$ A \cup B = \{0,1,2,3,4\} $$

The union of $$A$$ and $$B$$ contains everything that is either in $$A$$ or in $$B$$. Notice that this will include every element only once, since sets know only unique elements. That means, nothing will change if we also union the set $$D$$, since all elements are already included.

$$ A \cup B \cup D = \{0,1,2,3,4\} $$

### Intersection

Intersections allow us to find the elements that are overlapping in two or more sets. Meaning, all elements that are contained in all of the sets. Here is an example:

$$ A \cap B = \{2\} $$

This means all elements that are in $$A$$ and also in $$B$$. Notice, that this will reduce the number of elements in our case. If we now also intersect with $$D$$, this will leave us with an empty set. Since none of the elements are in all three sets.

$$ A \cap B \cap C = \emptyset $$

### Complements

Everything in the Universe that are not contained in A

$$A'$$

### Difference

Elements of set B that are not in set A

$$ A \setminus B $$

