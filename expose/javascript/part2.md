1. Line 12 prints 3 because `i` has function scope and thus retains its final value, which is `prices.length = 2`
2. Line 13 prints 150 because `discountedPrice` has function scope and thus retains its final value, which is `prices[2] * (1 - discount) = 300 * 0.5 = 150`
3. Line 14 prints 150 because `finalPrice` has function scope and thus retains its final value, which is `Math.round(discountedPrice * 100) / 100 = 150 * 100 / 100 = 150`
4. The function will return `[50, 100, 150]` because as each item price was halved, their value was pushed into the returned array
5. Line 12 causes a `ReferenceError` because `i` has block scope and therefore does not exist in line 12
6. Line 13 causes a `ReferenceError` because `discountedPrice` has block scope and therefore does not exist in line 13
7. Line 14 prints 150 because the print statement is in the same block as the declaration, and hence `finalPrice` takes on the value of the final item's half price
8. The function will return `[50, 100, 150]` because as each item price was halved, their value was pushed into the returned array, just like if the variables were declared with `var`
9. Line 11 causes a `ReferenceError` because `i` has block scope and therefore does not exist in line 11
10. Line 12 prints 3 because the `length` is within scope and always holds the length of `prices`, which is 3
11. The function will return `[50, 100, 150]` because as each item price was halved, their value was pushed into the returned array, just like if the variables were declared with `var` and `let`
12. Syntax
    1. `student.name`
    2. `student["Grad Year"]`
    3. `student.greeting();`
    4. `student["Favorite Teacher"].name`
    5. `student.courseLoad[0]`
13. Arithmetic
    1. `'3'+2` is 32 because 2 gets converted into a string and concatenated
    2. `'3'-2` is 1 because '3' gets converted into a number and is subtracted from
    3. `3+null` is 3 because `null` gets converted to 0 and is added
    4. `'3'+null` is '3null' because `null` gets converted to 'null' and concatenated
    5. `true+3` is 4 because `true` gets converted to 1 and added
    6. `false+null` is 0 because both `false` and `null` are converted to 0 and added
    7. `'3'+undefined` is '3undefined' because `undefined` gets converted to a string and concatenated
    8. `'3'-undefined` is `NaN` because '3' is converted to a number and `undefined` is `NaN`
14. Comparison
    1. `'2'>1` is true because 2 gets converted to a number
    2. `'2'<'12'` is false because this is a string vs. string comparison, and 1 is lexicographically before 2
    3. `2=='2'` is true because these values are equal after type conversion
    4. `2==='2'` is false because these values are not identical before type conversion
    5. `true==2` is false because `true` gets converted to 1
    6. `true===Boolean(2)` is true because `Boolean(2)` gets converted to `true` according to its numerical conversion rules
15. `==` checks for equality after type conversion, `===` checks for absolute identicality before type conversion
16. Code is in the proper file
17. `[2,4,6]` will be the result. Within the `i` indexed for loop, every element of the input array will be sent as input to the callback function (in this case, `doSomething`) and get doubled before being pushed into `newArr`. Hence, `newArr` is returned as the element-wise doubling of the input array.
18. Code is in the proper file
19. `1 \n 4 \n 3 \n 2`