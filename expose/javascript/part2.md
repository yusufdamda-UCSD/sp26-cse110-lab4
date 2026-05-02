### 1. What will happen at line 12 and why? If the code causes an error, explain why

Line 12 will print: 3 
This is because 'var' in this case is function scoped as opposed to block scoped. Even those 'i' is declared inside the loop it is still accessible outside the loop. After the loop is done, 'i' becomes 3. That's why 3 gets printed.

---

### 2. What will happen at line 13 and why? If the code causes an error, explain why.

Line 13 will print: 150 

This happens becuase 'discountedPrice' was declared with 'var', so it is accessible outside the for loop. After the for loop finishes, it has the value which is 300*(1-0.5) = 150.

---

### 3. What will happen at line 14 and why? If the code causes an error, explain why.

Line 14 will print: 150 

finalPrice was declared outside the loop with var, so it keeps getting updated each iteration. After the loop finishes, it holds the last value, which is 150.

---

### 4. What will this function return? Give a brief explanation why. If the code causes an error, explain why.

The function will return: [50, 100, 150]

Each price gets multiplied by (1 - 0.5), so everything in that is cut in half. The loop goes through all the values and pushes each finalPrice into the discounted array, which is returned at the end.

---

### 5. What will happen at line 12 and why? If the code causes an error, explain why.

This will cause an error 

'i' was declared with let inside the for loop so it only exists inside that loop. Line 12 is outside the loop, so it can’t access 'i', leading to a ReferenceError.

---

### 6. What will happen at line 13 and why? If the code causes an error, explain why.

This will cause an error because:

discountedPrice was declared with let inside the loop so it only exists in that place. Line 13 is outside the loop, so it can’t access it which causes a ReferenceError.

---

### 7. What will happen at line 14 and why? If the code causes an error, explain why.

Line 14 will print: 150 because:

finalPrice was declared outside the loop with let so it’s still accessible after the loop. It keeps updating each iteration, so after the loop it holds the last value, which is 150.

---

### 8. What will this function return? Give a brief explanation. If the code causes an error, explain why.

The function returns: [50, 100, 150] 

Each price is multiplied by (1 - 0.5) meaning everything is cut in half. The loop pushes each result into the array and then returns it.

---

### 9. What will happen at line 11 and why? If the code causes an error, explain why.

This will cause an error

i is declared with let inside the for loop so it only exists inside that loop. Line 11 is outside the loop, so it can’t access i, which leads to a ReferenceError.

---

### 10. What will happen at line 12 and why? If the code causes an error, explain why.

Line 12 will prints: 3

In the fucntion length was declared with the keyword 'const' outside the loop, so it is accessible there. Since the array has 3 elements, it prints 3.

---

### 11. What will this function return? Give a brief explanation. If the code causes an error, explain why.

The function returns: [50, 100, 150]

Each value in the array gets multiplied by (1-0.5) so everything is cut in half. The loop pushes each of the results into the discounted array, which is then returned by that function.

---

### 12. Given the above Object, write the notation for:  (These should be in your part2.md)

A. student.name

B. student['Grad Year']

C. student.greeting()

D. student['Favorite Teacher'].name

E. student.courseLoad[0]

---

### 13.

A. '3' + 2 = '32'  
The 2 in this case will turn in a string. The '+' with a string does concatenenation. 

B. '3' - 2 = 1  
In this case the string will become a number so that's why we get 1. 

C. 3 + null = 3  
In this case null will behave like 0. 

D. '3' + null = '3null'  
since we have '3' as a string, the null will behave like a string and get concatenated.

E. true + 3 = 4  
true becomes 1 so that means when you add it with 3 it will become 4.

F. false + null = 0  
false becomes 0 and null becomes 0.

G. '3' + undefined = '3undefined'  
undefined gets treated like text because of the string +.

H. '3' - undefined = NaN  
undefined cannot be turned into a useful number here.

---

### 14.

Comparison

A. '2' > 1 = true  
'2' gets converted to the number 2.

B. '2' < '12' = false  
Both are strings, so Javascript compares them like text. Since 2 comes after 1, it is false.

C. 2 == '2' = true  
== allows type conversion, so '2' becomes 2.

D. 2 === '2' = false  
=== will check the type too. One number is a string while the other is a number so wee will get false.

E. true == 2 = false  
true becomes 1, and 1 is not equal to 2.

F. true === Boolean(2) = true  
Boolean(2) becomes true, so both sides are true booleans.

---

### 15. Difference between == and ===

the == will compare values but also allows for type conversion. === compares both the value and type, meaning it is stricter and ususally the safer bet.

---

### 17

The result will be:
[2, 4, 6]

modifyArray goes through [1,2,3] and runs the callback on each value. doSomething just multiplies by 2, so 1 -> 2, 2 -> 4, 3 -> 6. Those values get pushed into a new array and returned.

---

### 19

Output:
1
4
3
2

1 and 4 run right away.  
3 runs next because setTimeout with 0 still waits a bit.  
2 runs last because it has a 1 second delay.