# Beginning Student Language (BSL) Syntax
#### Goal
- to write express that operates primitive data
- to write constant and function definitions
- to write step by step evaluation of expressions
- to use stepper to automatically step through the evaluation of an expression
- Use Dr Racket help desk

### *Expressions:* 
(+ 3 4) => 7  
(+ 3 (* 2 3) => 9  
(/12 (* 2 3)) => 2  
(sqr 3) => 9  
(sqrt 16 => 4  
(Operator (Expression)) => Value  
  
#### Excercise 1:
![Excercise 1](https://github.com/khongminhtn/computer-science-studies/blob/main/core-cs-programming/how-to-code-simple-data/Excercise1.png)  
Solution = 5  
  
However, when (sqrt 2) => #i1.4142135623730951. The ouput of the square root 2 is irrational number. (sqrt 2) takes infinite space to write number down, but the memory of a computer is finite so it uses symbols such as #i to indicate infinity and that it is a close estimation of actual output.

#### How BSL expressions works:
(operator operands)   
where () is a call to a primitive to operator followed by the operands  
 
BSL Evaluation  
1. Reduce operands(expresions) to values(single number).
2. Then apply primitive(operator) to the values(single number).
Intuitively evaluates from left to right, inside to outside  
 
### *Strings & Images*
 
Strings are represented in double quotes "" with primitive operations:
- (string-length "string")
- (substring "string") *zero based indexing*
- (string-append "string" "string")
 
Vector images expressed in the following:   
(circle 10 "solid" "red") such that:  
() is primitive call  
circle is operation  
values: 10, "solid", "red" - are values for operation to be applied  
 
### *Constant definition*
(define WIDTH 400) where (define name expression)  
WIDTH is now evaluates to 400  
such that (+ WIDTH + 2) => 402  
with *constants* it can only be defined once.  
> The use of constant is incredibly important as it provides code readiblity and ease of change.
 
### *Functions*
Function definitions help with DRY principle.  
Syntax:
```
(define (bulb c)  
    (circle 40 "solid" c))

where
(define (<function name> <parameter name>)
    (<expression>))

function call
(<function name><expression>)

with similarities
(<operator/primitive> <operands>)
```
Codes become clear and concise when function is invoked.  
Primitives evaluates as follows:
1. Reduce operands to single value
2. Apply primitive to value
 
Function evaluates as follows:
1. Reduce operands to single value
2. Replace expression of the function with the parameters that is now a value of a reduced operands
 
### *Booleans and If expressions*
Uses usual operators > < = true false.  
If expressions:
```
(if <expression>  question to evaluate
    <expression>  true answer
    <expression>) false answer

(and (<expression>, <expression>, ...) all has to be true, else false.
     <expression>
     <expression>)
```
IF expression evaluation:
1. if question expression is not a value, evaluate to get value and replace with value.
2. if the question evaluate to true, replace entire if expression with true answer expression.
3. if the question is false, replace entire if expression with false expression.
4. if question evaluates to neither true or false then produce error.
