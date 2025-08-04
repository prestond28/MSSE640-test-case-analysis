# Test Case Analysis - Pairwise testing

## Introduction

Pairwise testing is a testing technique that tests every input parameter pair combination possible. This way, you aren't testing every single input combination, but you are testing every combination of pairs. You don't get full test coverage this way, but it is a great way to still get a lot of coverage while decreasing the number of tests needed.

## Table / Diagram Example

Say you had these 4 input parameters and their potential values:

- A: 1, 2
- B: X, Y
- C: Red, Blue
- D: On, Off

Instead of having a table that includes all combinations of input values (which would make 16 test cases), you can use pairwise testing to make the table down to only 6 test cases, this way each pair of input values is tested at least once.

| Test Case | A | B | C   | D   |
|-----------|---|---|-----|-----|
| 1         | 1 | X | Red | On  |
| 2         | 1 | Y | Blue| Off |
| 3         | 2 | X | Blue| Off |
| 4         | 2 | Y | Red | On  |
| 5         | 1 | X | Blue| Off |
| 6         | 2 | Y | Blue| On  |

## When Testing Should Occur

This testing is great for if you have a large number of possible input values and want to make sure you get the most coverage you can, but don't necessarily have the resources available or it just wouldn't be feasible to test every combination of the full data set. 

## Limitations

The biggest limitation of this type of testing is that you can be missing coverage if there are important interactions that happen with three or more of the parameter values. Going along with this, if the program logic is too complex, you may be missing coverage on important logic that requires a specific combination of input values.

## AI Discussion

- No hallucinations. I love github copilot! (it's using the GPT-4.1 model)
- Site used to verify AI output: https://www.geeksforgeeks.org/software-engineering/pairwise-software-testing/
- One prompt I used: "what are the limitations of pairwise testing?"
