### 1. What is printed by line 9? If the code returns an error, explain why. ^^^^^

line 9 will print: value added: 20

This is because 'add' is true, so if the block runs and 'result' is assigned 'num1 + num2', which when added equals 20

---

### 2. What is printed by line 13? If the code returns an error, explain why.

Line 13 will print:
final result: 20

This works because 'var' has function scope, so the variable 'result' is accessible outside the if block even though it was declared inside it.

---

### 3. Why should you not use var? Explain why.

You shouldn’t use 'var' because it ignores block scope and can be accessed outside of where you define it, which can cause confusing bugs. It makes the code harder to track and debug. Using 'let' or 'const' is better since they stay within the block and behave more predictably.

### 4. What is printed by line 9? If the code returns an error, explain why.

Line 9 will print: 'values added: 20'

Since 'add' is true, and the if block runs and result becomes 10 + 10 = 20.

---

### 5. What is printed by line 13? If the code returns an error, explain why.

This causes an error.

Result was declared with let inside the if block, so it only exists there. Line 13 is outside the block, so it can’t access result, which leads to a ReferenceError.

---

### 6. What is printed by line 9? If the code returns an error, explain why.

This will cause an error. result is declared with const, so that means that it can't be reassigned. The line 'result = num1 + num2' tries to change its value. That ultimately will throw a TypeError before the program can even run lin 9.

---

### 7. What is printed by line 13? If the code returns an error, explain why.

This will not print anytrhing because the code had errors from the earlier lines. That means line 13 never executes. 
