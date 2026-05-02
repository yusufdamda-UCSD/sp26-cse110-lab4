## 1. What was the bug?

The bug/error was that num1 and num2 were strings so instead of adding them as numbers JavaScript concatenated them.

## 2. How would you fix it?

Convert them into numbers before we add them. 
let result = Number(num1) + Number(num2);