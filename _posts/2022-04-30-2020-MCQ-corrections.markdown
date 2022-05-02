---
layout: post
title:  "2020 MCQ Corrections"
categories: jekyll update
---

| Q# | Reasoning                |
|----|--------------------------|
| 1  | (3 + 2*3) = 6; (4 + 3/2) = 5; (7%4 +3) = 6; 9 + 5 + 6 = `20.0` |
| 5  | E causes the error, because a constructor with the same parameters in the same order already exists. I thought the question was asking about *replacing* the current constructor |
| 6 | Casts apply to the first value in the definition, so in `i = (double) 2 / 4 + 3` the cast applies to 2, making it 2.0; Then that leads to the expression becoming 0.5 + 3. |
| 7 | First clause b1 retains true if between 0 to 100; Else clause, b1 retains true if less than -100. This boolean expression does the same: `boolean b2 = (num < -100) || (num > 0 && num < 100);`|
| 11 | Loop will still go through when num == 1; meaning that num becomes 0 after `num--` and it will print `0` |
| 13 | `!(a && b) || c`, by DeMorgans law: `!a || !b || c` |
| 14 | Read the answer choices wrong, didn't realize the last option was `returning` the string, I thought it was just still assigning the string to the variable, in which case it would be overwritten and return the wrong output.  |
| 16 | There was a recursive call to itself right before it ran through the loop, I misinterpreted it as just a decrement. So it would fully decrement itself before running through all the loops that were "backed up".  |
| 21 | Worked out iterations: [link](https://pastebin.com/rh1mgztA) |
| 22 | Line 12 is executed each time the variable sm is updated because a new smallest value is found. When j has the value 0, sm is updated for "day" and "of". When j has the value 1, sm is updated for "of". When j has the value 4, sm is updated for "year". When j has any of the values 2, 3, or 5, sm is not updated. Line 12 is executed four times |
| 25 | Worked out iteration: [link](https://pastebin.com/09MjRuP5) |
| 26 | There are m * n iterations of the for loop in code segment I. In code segment II, the outer loop executes m times and the inner loop executes n - 1 times for each iteration of the outer loop. There are m * n - m iterations of the inner loop in code segment II, so "A" is printed m more times than "B" is printed. |
| 28 |  The method abMethod(String a, String b) removes all non-overlapping occurrences of string b from string a and returns the resulting String. It does this by repeatedly setting x to the index of an occurrence of b in a, then assigning a the result of the concatenation of the parts of a before and after the occurrence of b. The method call abMethod("sing the song", "ng") removes all occurrences of "ng" from "sing the song", returning "si the so". |
| 29 | 16 + { 8 + { 4 + {2 + {1 + {10} } } } } = 41 | 
| 31 | II won't go through everything in the array and III will throw error, so I is the only one left |
| 32 | Should just print "B," pretty simple but I guessed this question b/c I was running out of time |
| 33 | Iterations worked out [link](https://pastebin.com/vDpaJ34f) |
| 34 | numList.remove(i) removes an item from the list, which changes the size of the numList and messes with index positions. |
| 36 | This is honestly a really stupid problem, IDK how I'm supposed to recognize this relationship in 1.5 minutes and answer the question. Here is the CollegeBoard explanation: `The body of the for loop in methodOne is executed a / b times. The body of the while loop in methodTwo is executed a / b times only when a % b is equal to 0. When a % b is not equal to 0, the body of the while loop in methodTwo is executed an additional time. For example, when a has the value 11 and b has the value 5, a / b evaluates to 2 and the for loop is executed two times but the while loop is executed three times.` |
| 37 | num1 is being incremented by num2 and num2 is being incremented by 1 until num2 is == num3-1; Answer is `E` |
| 39 | worked out [answer](https://pastebin.com/mXRxh2cD) |
| 40 |At compile time, methods in or inherited by the declared type determine the correctness of a non-static method call. In line 1, obj1 is declared as an object of type A. Therefore, at compile time, there must be a message method in class A or its superclass. If the message method in class A is removed, the statement in line 3 will no longer compile. |