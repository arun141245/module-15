# Ex. No: 15c - Build a Heap Tree Using Python

## Aim
To write a Python program to build a heap tree using appropriate Python package and function.


## Algorithm
---
Start the program.
Import the heapq module.
Define a function heaptree(H) that takes a list H as input.
Use heapq.heapify(H) to convert the list into a min-heap.
Print the created heap.
End the program.

---

## Program

```
from binarytree import heap,build,Node
def heaptree(L):
  x=L
  t=build(x)
  for i in t.values:
    print(i,"-->",end='')
  print("\nHeight : ",t.height)
  print("Is min heap? : ",t.is_min_heap)
  print("Is complete tree? : ",t.is_complete)


```

## OUTPUT
<img width="1183" height="283" alt="image" src="https://github.com/user-attachments/assets/aff32a94-4865-454b-8b60-ac2627e64f51" />


## RESULT
Therefore, the output is the example to write a Python program to build a heap tree using appropriate Python package and function.
