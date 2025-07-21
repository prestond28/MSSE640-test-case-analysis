# Test Case Analysis - Equivalence Classes

## Introduction

Equivalence classes are input values that are grouped together based on their similarity and their expectations to produce the same output. For example, for the triangle program that checks 3 inputs and outputs a type of triangle, you could expect 1 1 1, 2 2 2, 3 3 3, ...999 999 999, and all the numbers beyond to be in the same equivalence class, because all of those inputs should output the same thing, an equilateral triangle.

## Table / Diagram Example

| Equivalence Class        | Example Input     | Expected Output     |
|--------------------------|-------------------|---------------------|
| All sides equal          | 3, 3, 3           | Equilateral         |
| Two sides equal          | 4, 4, 5           | Isosceles           |
| All sides different      | 3, 4, 5           | Scalene             |
| Invalid (zero/negative)  | 0, 4, 5           | Invalid Triangle    |
| Not a triangle           | 1, 2, 3           | Invalid Triangle    |

## When Testing Should Occur

Equivalence classes testing should occur when you have large data sets or an infinite amount of numbers that can be easily grouped into a few classes. Take the triangle program as a great example. This way, the whole data set can have test coverage without running the whole data set through the testing program, which could cost a lot of resources and unneeded effort.

## Limitations

Because equivalence classes testing groups similar data together and assumes the whole group will have the same outcome, it is possible to have holes in your testing because not every data point is being tested. So this type of testing should not be used if there is any question that your similar data could potentially produce different results.

## AI Discussion

- I used Github Copilot as my AI tool, and it did a great job at explaining equivalence classes. I didn't experience it hallucinate at all.

- Site used to validate AI output: https://www.geeksforgeeks.org/software-engineering/equivalence-partitioning-method/

- I asked "can you give me a table or diagram with example code or data?" (after I asked it to explain equivalence classes) And that is how I got the table with example data! It's pretty cool that it used my triangle program as an example just based on what I had already typed in the introduction and my previous conversations. The table it provided definitely helped my understanding of equivalence classes with a nice visual.