# Systematic Program Design
> ‘What do you want to program ?”
> “How do we break the problem ?”

## Design Method:
- Used to with any programming language.
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
 
**HtDF Recipe:**
1. Signature, purpose and stub.
2. Define examples, wrap each in check-expect.
3. Template and inventory.
4. Code the function body.
5. Test and debug until corrent.
 
**Example problem and solution**  
![HtDF Problem](https://github.com/khongminhtn/computer-science-studies/blob/main/core-cs-programming/how-to-code-simple-data//images/HtDF-problem.png)  
 
Solution:
1. Stub: consumes a number and produce a number.
    - Number -> Number.