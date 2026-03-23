# Ex. No: 15c - Build and Evaluate an Expression Tree

## Aim
To write a Python program to build and evaluate the given Expression tree.

## Algorithm
---
Start the program.
Create nodes for operators and operands.
Build the expression tree by connecting nodes in the correct hierarchical structure.
Define a recursive function evaluate(root):
If the node is a number (leaf), return it.
Else, recursively evaluate left and right subtrees.
Apply the operator at the current node to the results.
Return the final result from the root node.
End the program.

---

## Program

```
from binarytree import build,Node
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
 # Write your code here
    if root is None:
        return 0
    
    if isLeaf(root):
        return float(root.val)
    
    x=evaluate(root.left)
    y=evaluate(root.right)
    return process(root.val,x,y)
    
l=['+','*',3,8,4]
root=build(l)
print("The value of the expression tree is",evaluate(root))

```

## OUTPUT
<img width="1187" height="191" alt="image" src="https://github.com/user-attachments/assets/a3378e37-647d-4da0-954f-12cf30000833" />

## RESULT
Therefore, the output is the example to write a Python program to build and evaluate the given Expression tree.
