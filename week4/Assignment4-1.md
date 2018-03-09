# Assignment 4: Postfix Expressions

### Question 1
This problem is adapted from C-6.22 in the textbook.

Postfix notation is an alternate format for writing mathematical expressions. If op is an operator, and exp1 and exp2 are expressions, instead of writing exp1 op exp2, we would write exp1 exp2 op. An interesting feature of this notation is that no parentheses are needed to communicate the order of operations, because there is only one order consistent with each expression.

As an example, the mathematical expression ((5 + 2) * (8 - 3)) / 4 would be written 5 2 + 8 3 - * 4 / in postfix notation.

Write a script to evaluate postfix expressions involving numbers and the four operators +,-,*, and /. Your solution should be based on a single stack (either array-based or link-based) and you should not use recursive function calls.

You may want to import the operator module, which provides the following methods corresponding to basic mathematical operators: operator.add, operator.sub, operator.mul, operator.truediv. For example, if you set f equal to operator.add, you can find the sum of exp1 and exp2 using f(exp1, exp2).

When you are done, evaluate the following postfix expressions. Please round your answer to the nearest hundredth decimal point (ie: 0.01): 

#### Postfix Expression #1:

5 2 + 8 3 - * 4 /

#### Postfix Expression #2:

4 2 8 / 5 2 + 2 * - +

#### Postfix Expression #3:

2 2 8 4 5 / 6 * * 3 4 / 5 * + + 5 - 2 * 10 + +
