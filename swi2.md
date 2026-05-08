# SWI 2

## algorithm

- an algorithm is a set of instructions leading to solving a problem
- it describes a way on how to complete a task both for humans and computers

## properties of algoritmhs

- finality - the algorithm must end after a finite amount of steps
- resolution - the algorithm either returns a result or alerts the user of no existing solutions
- determinism - same inputs result in same outputs
- input - clearly defined inputs
- generality - the algorithm solves a group of problems, not just one instance (x+y=z, not 1+2=3)
- correctness - always gives the required result
- efficiency - time and memory efficient

## types of algorithms

- computational - numerical/symbolical operations (ie. factorials)
- sorting - sorting data (bubblesort, quicksort)
- searching - element lookup in arrays
- ordering - similar to sorting
- iterational - uses loops (for, while)
- recursive - function calls itself for looping
- deciding - choice between sets of instructions based on varying conditions

## examples
### iterative factorial:

```
FUNCTION FactorialIter(n)
  if n < 0 then ERROR
  result <- 1
  for i from 2 to n do
    result <- result * i
  return result
```

### recursive factorial:

```
FUNCTION FactorialRec(n)
  if n == 0 then return 1
  return n * FactorialRec(n-1)
```