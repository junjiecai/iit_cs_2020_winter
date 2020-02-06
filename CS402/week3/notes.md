# Week3 Notes

# Locality of reference
* temporal
A item in the cache is accessed now, chances are it will be accessed soon (Loop)
* spatial
A item is access now, its neighbour will be accessed next
    * code layout
    * data array
    
# Computing time for a program
Three parts
* CPU time (Time executing the instructions of your code)
* I/O time
* System time

## CPU time
cpu time  = IC(instruction executed count) * CPI(average clock cycle per instruction) * T_ck

Some instruction are simple, some are complicated.

CPI  = $\sum_{i=1}^n CPI_i * f_i$

|Class|$CPI_i$|$f_i$|
|---|---|---|
|Arithmetics/logic|2|60%|
|load|4|30%|
|Branching|4|10%|

CPI = 2*0.6 + 4*0.3 +5*0.1 = 2.9

Take Home:
Assuming a design team contemptuous tow changes to a perform?? design

the change would increase the number of arithmetic/logic instruction by f%(f=1)

and decrease at the same time the clock cycle by g%(g=8) percent

Should the team preceed with the changes?

 
 
# Instruction set design
 
operand + o or more address
* operand: what to do?
* o or more address: what to do with and what data to use

instruction classification
* 0 address ISA(aka instruction set architecture) (stack)
* 1 address ISA (aka accumulator)
* \>2 addresses ISA (usually has names) add
example:```add $t1, $t2, $t2```(MIPS)
 * add: operation
 * $t1: destination
 * $t2, $t2: data
 
*Important: This classification is based on a typical arithmetic/logic instruction in the instruction set*

## 1 address ISA (aka accumulator)
instruction format: 
op src # ACC <- ACC op src 
 
 
 
 