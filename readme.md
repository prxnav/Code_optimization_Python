#Python based Code Optimization

Python implementation of a simple compiler optimization technique called constant folding and dead code elimination.

The program reads in a file named "input.txt" containing the code to be optimized. It then performs constant folding, which is the process of simplifying constant expressions at compile-time. In this case, it looks for expressions involving two operands and an operator (e.g. "a + b", "c \* d") where both operands are constants (i.e. numeric literals) and evaluates the expression to a constant result (e.g. "a + b" becomes "c"). If one of the operands is a variable whose value has already been computed and stored in a dictionary, it substitutes that value and evaluates the expression. The program prints out the result of each constant folding operation.

After constant folding, the program performs dead code elimination, which is the process of removing code that does not contribute to the final output of the program. In this case, it looks for assignments to variables that are never used in subsequent code, and eliminates those assignments. The program prints out the resulting optimized code.
