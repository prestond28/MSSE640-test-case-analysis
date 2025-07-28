# Test Case Analysis - Decision Tables

## Introduction

Decision tables are a way to visualize which decisions a program can make based on certain conditions. They help you to analyze the decision making of the program and can help you determine if there are any holes in the logic in an organized and thorough way. Most decision tables list all of the possible combinations of inputs (if feasible) and then associate those combinations with the desired outcome.

## Table / Diagram Example

Here's a simple example we can all understand, since most programs need to have a user login:

| Condition         | Rule 1 | Rule 2 | Rule 3 | Rule 4 |
|-------------------|--------|--------|--------|--------|
| Username valid    |   Y    |   Y    |   N    |   N    |
| Password valid    |   Y    |   N    |   Y    |   N    |
| **Action**        |        |        |        |        |
| Allow login       |   X    |        |        |        |
| Show error        |        |   X    |   X    |   X    |

- Y = Yes, N = No, X = Action taken

In the table above, it lists all possible combinations of inputs and associates that with the action the program should take as the result.

## When Testing Should Occur

This testing is probably most helpful when you have complicated combinations of user inputs and need to lay them all out in an organized way. With complex conditions, it's possible to miss some that aren't normally thought about, but with a decision table, it forces you to write all the combinations out and think about the desired outcome.

## Limitations

Although decision tables work well for complex data combinations, it can also be difficult to manage if you have too much complexity. If you have an almost infinite amount of possible user inputs and therefore an almost infinite amount of possible combinations that can lead you to an almost infinite amount of possible outcomes, it wouldn't be feasible to have a giant table that goes on forever with all of that data. Especially when anything changes in the program, keeping that table updated would be a nightmare.

## AI Discussion

- I used Github Copilot for this assignment, and once again it did a great job at explaining everything without hallucinating.

- These are two sources I used to check the validity of the output it gave me:

https://www.geeksforgeeks.org/software-engineering/software-engineering-decision-table/

https://www.browserstack.com/guide/decision-table

- I liked the example it gave me on one of the previous assignments when I prompted it by asking for an example table, so I asked it again for an example table, and it did not disappoint! The example tables it gives me always help deepen my understanding of the subject. I ended up using the table it gave me in my assignment.