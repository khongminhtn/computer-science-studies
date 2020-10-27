# Systematic Program Design
> ‘What do you want to program ?”
> “How do we break the problem ?”

### Design Method:
- Used to with any programming language
- Manages complexity:
  - Solve 1 problem at a time
    - Easy to think
    - Easy to read
    - Easy to modify

#### Design Method = From poorly formed -> Well-structured solution


### Part 1: Beginning Student Language (BSL)
#### Goal
- to write express that operates primitive data
- to write constant and function definitions
- to write step by step evaluation of expressions
- to use stepper to automatically step through the evaluation of an expression
- Use Dr Racket help desk

#### Expressions: 
( + 3 4) => 7  
(+ 3 (* 2 3) => 9  
(/12 (* 2 3)) => 2  
(sqr 3) => 9  
(sqrt 16 => 4  
(Operator (Expression)) => Value  
  
#### Excercise 1:
![Excercise 1](https://github.com/khongminhtn/computer-science-studies/blob/main/core-cs-programming/how-to-code-simple-data/Excercise1.png)  
Solution = 5  
  
However, when (sqrt 2) => #i1.4142135623730951. The ouput of the square root 2 is irrational number. (sqrt 2) takes infinite space to write number down, but the memory of a computer is finite so it uses symbols such as #i to indicate infinity and that it is a close estimation of actual output.

**How BSL expressions works:**
(operator operands)   
where () is a call to a primitive to operator followed by the operands  
 
BSL Evaluation  
1. Reduce operands(expresions) to values(single number).
2. Then apply primitive(operator) to the values(single number).
Intuitively evaluates from left to right, inside to outside  