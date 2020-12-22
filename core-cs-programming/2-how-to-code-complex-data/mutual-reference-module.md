# Mutual Reference Module  
 
### Learning Goals
-   Able to identify problem domain information of arbitrary size represented using arbitrary arity trees
-   Able to use design recipes to design with arbitrary arity trees
-   Able to use the design recipes with mutually referential data.
-   Able to predict and identify the correspondence between external, self, mutual reference in data definitions and calls, recusion and mutual-recursion in functions that operate on data.
 
### Mutually recursive data  
New Form of Data -> Arbitrary arity tree (most complex)  
A List is a 1 dimensional arbitrary sized data, whereas a Arbitrary arity tree is a 2 dimensional List.  
 
Working with 1 dimensional List we have 1 recursive cycle  
Working with 2 dimensional List we have 2 recursive cycles  
 
When designing functions that operates on mutually recursive types, you design multiple function at once