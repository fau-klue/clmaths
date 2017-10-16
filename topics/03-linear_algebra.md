---
layout: default
title: Linear Algebra
description: "A brief introduction into Linear Algebra"
---

# Linear Algebra

Linear algebra is the heart and soul of deep learning algorithms in machine learning. This course will give you a good, and hopefully intuitive, knowledge of vectors and matrices. These concepts are key to many theories in computational linguistics, some of which we will mention in the chapter.

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

We can now represent each document (measurement/data point) as a vector with three values.

$$ text1 = \begin {bmatrix} 132 \\ 231 \\ 321 \end{bmatrix} $$

To specify one specific element in a vector we use an index, just like in programming languages when we want to get a specific element of an array. Note that indices here start at 1.

$$ text1 _ 1 = 132  $$

$$ text1 _ 2 = 231  $$

### Matrix

Matrices are two-dimensional fields of numbers, denoted with an upper case letter:

$$ M = \begin{bmatrix}a & b & c\\d & e &f\end{bmatrix} $$

This matrix has a dimensions of $$2 \times 3$$, since it has two rows and three columns. This dimensions are usually denoted by $$ m \times n $$ or, in case of a square matrix $$ m \times m $$.

Like before, we look at matrices from a data science perspective. Looking back at our table with text documents, we have already seen a matrix. The table can be rewritten as a matrix like so:

$$ D = \begin{bmatrix}132 & 231 & 321 \\ 222 & 321 & 132\end{bmatrix} $$

Each row representing a document (measurement/data point). Again, to specify one specific element in a matrix we use indices, this time however we need two values since we have a two-dimensional field.

$$ D _ {1,1} = 132 $$

$$ D _ {2,1} = 222 $$

### Tensor

Tensors are Matrices with more then two dimensions. We can imagine a three-dimensional tensor as a stack of matrices in a grid. In a three-dimensional tensor we would have to use three indices to access a specific element.

$$ D _ {i,j,z} $$

## Operations

There are several operations defined on all of the components above. Here we will focus on matrix operations, since these are commonly found in fields like Machine Learning.

### Transpose

The transpose of a matrix is a new matrix whose rows are the columns of the original.

$$ M = \begin{bmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{bmatrix} $$

$$ M ^T = \begin{bmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix} $$

### Scalar Multiplication

As we have seen, a scalar is just a single value. Multiplying scalars with a matrix means, multiplying every value in the matrix with the scalar. Let's see an example:

$$ 2 * \begin{bmatrix}3 & 8 \\ 7 & 5 \end{bmatrix} = $$

$$ \begin{bmatrix}2 * 3 & 2 * 8 \\ 2 * 7 & 2 * 5 \end{bmatrix} = \begin{bmatrix} 6 & 16 \\ 14 & 10 \end{bmatrix} $$

### Matrix Addition

Matrix addition means adding each value of a matrix $$A$$ to its corresponding value in a matrix $$B$$. Let' see an example to make this clear.

$$ A = \begin{bmatrix}2 & 5 \\ 1 & 3 \end{bmatrix} $$

$$ B = \begin{bmatrix}4 & 9 \\ 5 & 6 \end{bmatrix} $$

$$ A + B = \begin{bmatrix} 2 + 4 & 5 + 9 \\ 1 + 5 & 3 + 6 \end{bmatrix} = \begin{bmatrix}6 & 14 \\ 6 & 9 \end{bmatrix} $$

Note that the matrices need to have the same dimensions.

### Matrix Multiplication

Multiplication of two matrices means, multiplying the values of the row in matrix $$A$$ with the values of the column in matrix $$B$$, then adding them all up. This is called a Dot Product. Let us see and example to make this operation clear:

$$ A = \begin{bmatrix}2 & 5 & 2 \\ 1 & 3 & 3\end{bmatrix} $$

$$ B = \begin{bmatrix}1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix} $$

We now take the first row of $$A$$ and the first column of $$B$$, multiply each value and add them up:

$$ (2*1) + (5*2) + (2*3) = 18 $$

Then we take the first row and second column, then the second row and first column, and so on.

$$ A * B = \begin{bmatrix}18 & 45 \\ 16 & 37\end{bmatrix} $$

Note that the number of rows of the first matrices has to match the number of columns in the second. Hint: You can see if two matrices can be multiplied by checking if the inner dimensions align. In the example above the dimensions are $$2 \times 3$$ and $$3 \times 2$$.
