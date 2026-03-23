# Experiment 15e: Heap Tree

## Aim
To write a Python program to build a heap tree using appropriate Python package and function.

---

## Algorithm

1. Start the program.
2. Import the `heapq` module.
3. Define a function `heaptree()` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a valid heap (min-heap).
5. Print the created heap.
6. End the program.

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
<img width="1183" height="283" alt="image" src="https://github.com/user-attachments/assets/de9e613a-6350-4f43-9b63-8195507c9674" />

## RESULT
Therefore, the output is the example to write a Python program to build a heap tree using appropriate Python package and function.
