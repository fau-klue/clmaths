---
layout: default
title: Set Theory
description: "A brief introduction into Set Theory"
---

# Set Theory

This course will teach you some elementary Set Theory. We look at basic properties of sets, how to define a set, and how to compare different sizes of sets.

## Introduction

Sets can be found almost anywhere. Sets are considered to be subsets of a large universal set, called the universe. Contents of this universe will depend on the context. For example, we can define the universe as all humans on the planet, then take sets of these people and pick one person as an element of a set. All the words in a language can be seen as a set, a word as an element of it. Now for some formal definitions.

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

Enumerating all elements is possible for small sets, however if we have many (or infinite) elements in one set, we rather describe elements by their properties. For example, let us define a set of all natural numbers. Writing an extensional list of these numbers would take a long time, since they are infinite. We can avoid this by using an intentional description:

$$ N = \{ x \in U : x\ is\ an\ even\ number \} $$

This means, the set $$N$$ contains the elements $$x$$ from the universe $$U$$ that are a number and are even. More general we can say: For a property $$P$$ and an element $$e$$ of a set $$S$$, we write $$P(e)$$ to indicate that $$s$$ has the property $$P$$. Now we have the possibility to shorten our notation:

$$ A = \{e \in S : P(e)\} $$
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

The formal definition would be:

$$ A \cup B = \{ x \in U : x \in A\ or\ x \in B \}$$

### Intersection

Intersections allow us to find the elements that are overlapping in two or more sets. Meaning, all elements that are contained in all of the sets. Here is an example:

$$ A \cap B = \{2\} $$

This means all elements that are in $$A$$ and also in $$B$$. Notice, that this will reduce the number of elements in our case. We can use a Venn Diagram to visualize two intersecting sets:

<iframe width="100%" height="500" src="//jsfiddle.net/martialblog/9hw4bsvb/1/embedded/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

If we now also intersect with $$D$$, this will leave us with an empty set. Since none of the elements are in all three sets.

$$ A \cap B \cap C = \emptyset $$

The formal definition of the intersection would be:

$$ A \cap B = \{ x \in U : x \in A\ and\ x \in B \}$$

### Difference

The difference of two sets is defined as: All elements of set $$A$$ that are not in set $$B$$. Let's see an example to make this clear:

$$ A \setminus B = \{1,3\} $$

This means, exclude all elements from $$A$$ that are included in $$B$$. In our example this excludes the element $$2$$. Notice that the notation $$ A \setminus B $$ and $$ A - B $$ are equivalent.

The formal definition would be:

$$ A \setminus B = \{ x \in U : x \in A\ and\ x \notin B \}$$

### Complement

We can invert the meaning of a set by its complement. That means every element in the defined universe that is not contained in $$A$$. Notation differs, but complements are usually defined like this:

$$ Universe = \{1,2,3,4,5\}$$

$$ Z = \{1,2\} $$

$$ Z' = \{3,4,5\} $$

The formal definition would be:

$$ A' = \{ x \in U : x \notin A \}$$
