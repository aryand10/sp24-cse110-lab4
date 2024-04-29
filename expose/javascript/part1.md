# Part 1 JavaScript Questions
1) Line 9 prints 'values added: 20'.
2) Line 13 prints 'final result: 20'.
3) Line 9 prints 'values added: 20'.
4) Line 13 will result in a `ReferenceError` because the `let` declaration for `result` means that it is block-scoped and not accessible outside of the `if` block where it was declared. 
5) Line 9 will not be printed because a `TypeError` will be occur on line 7 since `result` is a `const` and constants cannot be reassigned which is what is attempted in line 7. 
6) Line 13 will not be printed because a `TypeError` will be occur on line 7 since `result` is a `const` and constants cannot be reassigned which is what is attempted in line 7. 
