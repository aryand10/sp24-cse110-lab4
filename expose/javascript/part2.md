# Part 2 JavaScript Questions
1) At line 12, the value of `i` will be printed which in this case is **3**, because the list is of length 3 and the for-loop will exit when `i` is set to the length of the list. An error will not occur because the `i` has a declaration of `var` which means it is function-scoped.
2) At line 13, the value of `discountedPrice` will be printed in which this case is **150** because that is the last value in the list multiplied by the value of the discount. An error will not occur because `discountedPrice` has declaration of `var` which means it is function-scoped.
3) At line 14, the value of `finalPrice` will be printed in which this case is **150** because that is the last value in the list multiplied by the value of the discount. An error will not occur because `finalPrice` has delcaration of `var` which meant it is function-scoped. 
4) This function will return the array `discounted`, which will be **[ 50, 100, 150 ]** in this case. This is the array of all the final prices of each item in the prices array once the discount has been applied by the function. An error will not occur because `discounted` and all necessary variables have `var` declarations which provide function-scope. 
5) Line 12 will result in a `ReferenceError` because `i` is declared using `let` which results in the variable only having block-scope within the `for`-loop. 
6) Line 13 will result in a `ReferenceError` because `discountedPrice` has a declaration of `let` inside the `for`-loop which means that is has block-scope within the `for`-loop only.
7) Line 14 will result in `finalPrice` being printed which in this case is **150**. Even though `finalPrice` is declared using `let`, the block it is defined in is the same block in which it is called so no errors occur. 
8) The function will return the array `discounted`, which will be **[ 50, 100, 150 ]** in this case. This is the array of all the final prices of each item in the prices array once the discount has been applied by the function. An error will not be thrown because `discounted` and all necessary variables have scope within their required blocks. 
9) At line 11 a `ReferenceError` will occur because `i` is decalred using `let` which results in the variable only having block-scope within the `for`-loop. 
10) At line 12, the `length` variable indicating the lenght of the array will be printed which in this case is **3**. There will be no errors because the `const` declaration on `length` is used properly since it is never reassigned. 
11) The function will return the array `discounted`, which will be **[ 50, 100, 150 ]** in this case. This is the array of all the final prices of each item in the prices array once the discount has been applied by the function. An error will not be thrown because `discounted` and all necessary variables have scope within their required blocks. 
12) See parts below
    1)  A) `student.name;`
    2)  B) `student['Grad Year']; `
    3)  C) `student.greeting();`
    4)  D) `student['Favorite Teacher'].name;`
    5)  E) `student.courseLoad[0];`
13) See parts below
    1)  A) Output: '32' Explanation: String concatenation performed converting 2 to a string resulting in '32'. 
    2)  B) Output: 1 Explanation: - results in numeric conversion of 3 so final result is 1. 
    3)  C) Output: 3 Explanation: null is converted to zero so the sum of 3 and zero is 3
    4)  D) Output: '3null' Explanation: String concatenation is peformed resulting in combined outcome '3null'. 
    5)  E) Output: 4 Explanation: True is treated as a 1 so the sum of 1 and 3 is 4
    6)  F) Output: 0 Explanation: False is treated as 0 so the sum of 0 and 0 is 0
    7)  G) Output: '3undefined' Explanation: String concategnation occurs so the combined result is '3undefined'
    8)  H) Output: NaN Explanation: the - results in arithmetic ocurring and undefined is changed to NaN in numeric contexts 
14) See parts below
    1)  A) Output: true Explanation: Numeric conversion/comparison performed so output is true
    2)  B) Output: false Explanation: Lexicographic comparison made character by character and '2' is greater than '1'
    3)  C) Output: true Explanation: Numeric conversion/comparison performed so output is true
    4)  D) Output: false Explanation: === does not result in any type conversion/coercion so string is compared to number and they are not equal
    5)  E) Output: false Explanation: true is converted to 1 and 1 is not equal to 2
    6)  F) Output: true Explanation: Boolean(2) is converted to true because any non-zero value is true 
15) When the `==` operator is used, type conversions are performed as necessary before any conversions are attempted to be made. When `===` is used, no type conversions will ever be peformed and the comparison will be made without any type conversion, returing false if objects are not the same type. 
16) Code can be found in part2-question16.js
17) The result of this call will be **[ 2, 4, 6 ]**. First, inside `modifyArray`, a new array `newArr` is created. Then, the `for`-loop starts with `i` being initialized to 0. The first element (1) is passed to `doSomething()`, which will return 2, which is pushed into `newArr`. The loop on the next iteration will increment to the second element (2), which is passed to `doSomething()`, which will return 4, which is pushed into `newArr`. The loop on the next iteration will increment to the third element (3), which is passed to `doSomething()`, which will return 6, which is pushed into `newArr`. Now that the loop is done, the final `newArr` is what is returned by `modifyArray`. 
18) Code can be found in part2-question18.js
19) The output of the code can be seen below. First, `console.log(1)` is called and logs 1. The first `setTimeout` function is called with sets up a timer to log 2 after 1 second. Then the second `setTimeout` function is called with sets up to log 3 as soon as possible but after the current script finishes. Then `console.log(4)` is called immediately but times out before being able to execute so 4 is logged. After the script is finished, the timmer events are handled which results in 3 being logged since it was queued first with its 0 second delay and then after 1 second the 2 is finally logged.
```
1
4
3
2
```