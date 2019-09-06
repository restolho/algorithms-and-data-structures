# Algorithms and Data Structures
<br>

This repository has several explanations of data structures and algorithms which are commonly used on tech interviews. There is also several solutions of coding problems from LeetCode. Many examples in this repo were taken from these two books. Buy them if you wish to know more about this subject.

- Cracking the Coding Interview, 6th Edition
- Grokking Algorithms

## Index
1. [Big O notation](#big-o-notation)
2. [Data Structures](#data-structures)
3. [Algorithms](#algorithms)

## Big O notation
<br>

The Big O notation is the metric to use when you want to describe the efficiency of an algorithm. Failure to understand this metric might result in a slow and not very efficient algorithm which could potentially have an impact on your application.

### A simple analogy
You have a file on a hard drive and you want to send it to a friend that lives in the other side of the country. The vast majority of people would just send it by email or some other electronic form. This sounds reasonable but only up to a certain point. If it's a small file, sure, you are probably doing the right thing since getting on a plane and going across the country could take several hours. But what if the size of the file is really large? Imagine the file size is 500TB. It's theoretically possible that getting on a plane could be faster than using the internet.

This is what Big O time means. It's possible to describe the data transfer algorithm runtime as:
- Electronic Transfer: O(n), where n is the file size.
- Airplane Transfer: O(1), if the file size increases, it will still take the same amount of time to deliver it.

### Algorithms running times growth

Imagine you are writing a search algorithm for a company. This algorithm needs to be fast and it only has 10 seconds to execute. Let's assume you have a sorted array of 100 numbers, if you use a simple search it could take you 100 guesses to find the correct number. 

Example:

I select the number 100. The algorithm starts searching on the arrays first position, it finds 1 and since 1 != 100 it moves on to the next position ... In this particular case it would take 100 guesses just to figure out the number selected. Let's assume that each guess takes 1ms. This algorithm would take 100ms to run.

What if we you Binary Search? (link to binary search) Instead of taking 100ms, it would only take us 7.

So can we assume that a simple search is roughly 15 times (7*15 = 105ms) slower than Binary search?

The answer is NO! Imagine that instead of an array with 100 sorted elements we would get an array with a.000.000.000. This would take the simple search algorithm 11 days to search but only 32ms using Binary Search.

You should know that the Big O notation gives you the rate of increase of a given algorithm. 

Another thing you should pay attention is that the Big O notation shows the worst possible case. Using the previous example, if I had picked the number 1 the simple search would have found the number right way O(1). However, we must show the worst possible case meaning O(n). Given this it's easily seen that a O(n) algorithm can actually run faster than O(1). Big O is meant to describe the rate of increase, for that reason we should drop constants. So an algorithm that runs in O(2n) is actually O(n). In addition to drop constants, you should also drop Non-Dominant terms. Example:

- O(n^2 + n) should be O(n)
- O(n + log n) should be O(n)

#### Common Big O run timea

- O(log n), also known as log time. Example binary search (link).
- O(n), also known as linear time. Example simple search.
- O(n * log n). Example: A fast sorting algorithm like merge or quick sort.
- O(n^2). Example: A slow sorting algorithm like selection sort.


## Data Structures
<br>

1. [Arrays](#arrays)
2. [LinkedLists](#linkedlists)
3. [HashTables](#hashtables)
4. [Stack](#stack)
5. [Queue](#queue)
6. [Trees](#trees)
7. [Graphs](#graphs)


## Algorithms
<br>

1. [Divide and Conquer](#divide-and-conquer)
2. [Dynamic Programming](#dynamic-programming)
3. [Greedy Algorithms](#greedy-algorithms)
4. [Graph Search](#graph-search)
