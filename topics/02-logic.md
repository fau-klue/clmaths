---
layout: default
title: Predicate Logic
description: "A brief introduction into Predicate Logic"
---

# Predicate Logic

Logic as a formal system can be used by linguistics compare and analyze natural language. This formal system can be defined very clearly and thus be also used in computer science, for example: In the field of Artificial Intelligence formal logic can be used for reasoning. We will look at some basic logic formalims and then briefly look at Lambda calculus.

## Introduction

In sentential (or propositional) logic sentences (or propositions) are the smallest unit, these sentences can either be *true* or *false*. This is called a **Boolean**, a variable that can only take on the values true or false. Usually variables are represented by single capital letters. Let us see some examples:

$$ M = The\ moon\ orbits\ earth $$

$$ E = The\ earth\ is\ flat $$

$$ M = True $$

$$ E = False $$

We can see that both these propositions can have a true or false (boolean) value.

## Operations

Furthermore, we can combine simple sentences to form more complex utterances. These combinations can be seen as operations on the propositions, returning again either true or false.

### Conjunction

The conjunction can be translated as the word "and". It yields true if both conjuncts are true and false if any of the conjuncts is false. Let us first define some sentences:

$$ S = Saturn\ has\ a\ ring = True $$

$$ J = Jupiter\ is\ a\ gas\ giant = True $$

$$ M = The\ moon\ is\ made\ of\ green\ cheese = False $$

Now we can perform a conjunction to combine these, changing the resuling boolean.

$$ S \land J = True $$

This translates to: "Saturn has a ring and Jupiter is a gas giant", which is true.

$$ M \land J = False $$

This translates to: "The moon is made of green cheese and Jupiter is a gas giant", which is false.

All operations have a so called "truth table", which shows the result given any input.

| $$A$$  | $$B$$  | $$A \land B$$  |
|:--:|:--:|:--:|
| True   | True  | True  |
| True   | False | False |
| False  | True  | False |
| False  | False | False |

### Disjunction

The disjunction can be translated as the word "or". It yields true if one of the disjuncts is true and is denoted by the $$ \lor $$ symbol.

The truth table for the disjunction:

| $$A$$  | $$B$$  | $$A \lor B$$  |
|:--:|:--:|:--:|
| True   | True  | True  |
| True   | False | True  |
| False  | True  | True  |
| False  | False | False |

### Negation

The negation can be translated as the word "not". It yields the opposite value of whatever input is given, true becomes false and vice versa. It is denoted by the $$\neg$$ symbol.

The truth table for the negation:

| $$A$$  | $$ \neg A$$  |
|:--:|:--:|
| True  | False |
| False | True  |

### Conditional

The condition, or implication, can be translated as "if ... then". It is denoted by the $$\rightarrow$$ symbol.

The truth table for the condition:

| $$A$$  | $$B$$  | $$A \rightarrow B$$  |
|:--:|:--:|:--:|
| True   | True  | True  |
| True   | False | False |
| False  | True  | True  |
| False  | False | True  |

Note, that from a false proposition, anything follows (ex falso quodlibet).

## Predicates

As we have seen, propositional logic is a rather blunt instrument, that can not seen beyond sentences. Predicate logic solves this problem by expanding the logic formalism we have looked at so far. It does so by using smaller units than sentences, its basic unit is an *entity*, which correspond to things in the real world. Futhermore, these entities have properties (predicates) assigned to them. Let see an example, let us define three simple entities:

$$ D = Dave $$

$$ H = Hal $$

New let us use simple predicates to give these entities some properties. Predicates are written in uppercase letters and use parenthesis to take arguments.

$$ ROBOT(H) $$

$$ HUMAN(D) $$

This will translate as: "Hal is a Robot" and "Dave is a Human". Predicates can also be actions:

$$ JOG(D) $$

This will translate as: "Dave jogs". As you can see we defined an intransitive verb as and action of an entity. This also applies to transitive verbs, in that case the predicate will take two arguments.

$$ LIKE(D, H) $$

This will translate as: "Dave likes Hal". The same way ditransitive verbs can be written as a predicate with three arguments:

$$ R = Report $$

$$ GIVE(H, D, R) $$

This will translate as: "Hal gives Dave the report".

## Quantifiers

## Lambda Calculus
