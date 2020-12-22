# Systematic Program Design
> ‘What do you want to program ?”
> “How do we break the problem ?”

## Design Method:
- Used to with any programming language.
- Make problem specific.
- Manages complexity:
  - Solve 1 problem at a time.
    - Easy to think.
    - Easy to read.
    - Easy to modify.

#### Design Method = From poorly formed -> Well-structured solution

#### Learning goals:
- Using How to Design Function (HtDF) recipe to design functions that operate primitive data.
- Read complete function design and identify its different elements.
- Evaluate different elements for clarity, simplicity and consistency.
- Evaluate the entire design to observe how well it solves a problem
 
HtDF recipe makes simple problems harder to solve, but makes complex problems easier to solve.  
 
## *HtDF Recipe*
**What is HtDF ?**  

- The HtDF recipe systematizes the design of a function.  
- Ensures high quality function.
- Well tested
- Makes hard problems easier to solve
  - Break problems down to smaller steps
- Makes easy problems a little harder to design
- Not intended for waterfall process (step by step/ procedural programming)
 
**HtDF Recipe:**
1. Signature, purpose and stub.
2. Define examples, wrap each in check-expect.
3. Template and inventory.
4. Code the function body.
5. Test and debug until corrent.
 
Each step helps/guides the resolution of step that precedes it.
 

 
**Example problem and solution**  
![HtDF Problem](https://github.com/khongminhtn/computer-science-studies/blob/main/core-cs-programming/how-to-code-simple-data//images/HtDF-problem.png)  
 
**Solution:**
Step 1: 
- Signature: what data does it consume and what data does it produce.
  - Number, String, Boolean ... => Boolean, String, Number...
- Purpose: 1 line description of what it produces given the consumption
- Stub: a correct definition of a function with the correct name and parameters and produces with a dummy result of correct type.
  - (define(name parameter1, parameter2,...) result)
 
Step 2:
- (check-expect (name expected-parameters) expected-results)
- examples should be enough to demonstrate the possible results and parameters
- look out for corner cases
 
Step 3:
- Outlines the function.
```
(define (double n)       | -> template
    (... n))             | -> n is what will be worked with
```
 
Step 4:
- The actual body of code of the function.
```
(define (double n)
    (* 2 n))             | -> code body       
```
Using all the information above as guidance to definet he code body.  
 
Step 5:  
- Run and check for any bugs.  
 
 

**Question:**  
![HtDF Problem](https://github.com/khongminhtn/computer-science-studies/blob/main/core-cs-programming/how-to-code-simple-data//images/HtDF-pratice.png)  
 
- Signature: string => string
- Purpose: pluralize a word
- Stub: (define (pluralize string) string)
- Check:
  1. (check-expect (pluralize burger) burgers)
  2. (check-expect (pluralize wing) wings)
- Outline:
```
(define (pluralize string)
  (... string))    where ... means do something
```
- Body:
```
(define (pluralize string)
  (string-append string s))
```
- Debug
