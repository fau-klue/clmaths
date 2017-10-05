---
layout: default
title: Linear Algebra
description: "A brief introduction into Linear Algebra"
---

# Linear Algebra

Linear algebra is the heart and soul of deep learning algorithms in machine learning. This couse will give you a good, and hopefully intuitive, knowledge of vectors and matrices. These concepts are key to many theories in computational linguistics, some of which we will mention in the chapter.

## Introduction

Let us begin by looking at the basic components of this chapter.

### Scalar

The simplest and probably obvious component is a single value, or scalar.

$$ a $$

### Vector

A vector is an arrangement of numbers, usually denoted by a lower case letter, written as a column like so:

$$ v = \begin{bmatrix}a \\ b \end{bmatrix} $$

Often, vectors are introduced an arrow in a two dimensional space. In computer/data science we think of vectors as an array, or one data point. Imagine a table in which we write down attributes of a text document. The attributes are the numbers of part-of-speech categories:

| Nouns  | Verbs  | Adjectives  |
|:--:|:--:|:--:|
| 132  | 231  | 321  |
| 222  | 321  | 132  |

We can now represent each document (mesurement/data point) as a vector with three values.

$$ text1 = \begin {bmatrix} 132 \\ 231 \\ 321 \end{bmatrix} $$

To specify one specific element in a vector we use an index, just like in programming languages when we want to get a specific element of an array. Note that indices here start at 1.

$$ text1 _ 1 = 132  $$

$$ text1 _ 2 = 231  $$

### Matrix

Matrices are two-dimensional fields of numbers, denoted with an upper case letter:

$$ M = \begin{bmatrix}a & b\\c & d\end{bmatrix} $$

Like before, we look at matrices from a data science perspective. Looking back at our table with text documents, we have already seen a matrix. The table can be rewritten as a matrix like so:

$$ D = \begin{bmatrix}132 & 231 & 321 \\ 222 & 321 & 132\end{bmatrix} $$

Each row representing a document (mesurement/data point). Again, to specify one specific element in a matrix we use indices, this time however we need two values since we have a two-dimensional field.

$$ D _ {1,1} = 132 $$

$$ D _ {2,1} = 222 $$

### Tensor

Tensors are Matrices with more then two dimensions. We can imagine a three-dimensional tensor as a stack of matrices in a grid. In a three-dimensional tensor we would have to use three indices to access a specific element.

$$ D _ {i,j,z} $$

## Operations

## Advanced Topics
