# Stack-in-C-Plus-Plus

Aim: To study the concept of Stack in C++ and implement operations like push, pop, and display.

Tools Used: VS Code or Programiz online compiler.

# Theory

# Stack in Cpp

A **stack** in C++ is a linear data structure that works on the **Last In, First Out (LIFO)** principle. It allows operations like **push()** to add elements, **pop()** to remove elements, and **top()** to access the last inserted element. Stacks can be implemented using **arrays**, **linked lists**, or the **STL stack container**. They are commonly used in **recursion, expression evaluation, and function call management**.

-Can be implemented using arrays or linked lists.
-Requires a pointer/index (top) to keep track of the top element.

# Program-1: Stack Implementation
This C++ program demonstrates the **implementation and basic operations of a stack** using an **array**. The `Stack` class defines an integer array `arr[MAXSIZE]` and an integer `top` to keep track of the stack’s current position. The **constructor** initializes `top` to -1, indicating an empty stack. The **push()** function adds an element to the top of the stack if space is available, otherwise it shows a “Stack Overflow” message. The **pop()** function removes the top element if the stack is not empty, else it displays “Stack Underflow.” The **display()** function prints all elements present in the stack.

In the `main()` function, elements are pushed and popped to perform arithmetic operations using the stack logic. First, numbers 1 and 2 are pushed, popped, and added to form 3, which is then pushed back. Next, 3 is pushed, and both 3 (sum) and 3 (new value) are popped and multiplied to form 9, which is pushed again. Finally, the **display()** function shows the result `9` as the final output. This illustrates how a stack can be used to perform **arithmetic and expression evaluations** following the **LIFO (Last In, First Out)** principle.

--> Algorithm:

1. Start
2. Initialize top = -1 and define MAXSIZE = 5.
3. Create a class Stack with functions:
  --push(data) → to insert an element.
  --pop() → to remove the top element.
  --display() → to show all elements in the stack.
4. In push(data):
  --If top < MAXSIZE - 1, increment top and store data in arr[top].
  --Else, print “Stack Overflow”.
5. In pop():
  --If top > -1, decrement top.
  --Else, print “Stack Underflow”.
6. In display():
  --Print elements from index 0 to top.
7. In main():
  --Create an object s1 of class Stack.
  --Push 1 and 2 onto the stack.
  --Pop 2 and 1, add them → result = 3.
  --Push result (3) onto the stack.
  --Push 3 again.
  --Pop the two 3s, multiply them → result = 9.
  --Push result (9) onto the stack.
  --Display the stack (output = 9).
8. Stop

# Conclusion
The program successfully demonstrates the implementation of a stack using an array in C++. It performs basic stack operations such as push, pop, and display while following the LIFO (Last In, First Out) principle. The arithmetic operations performed using the stack show how data can be efficiently managed and processed. This experiment helps understand how stacks work internally and how they can be applied in real-world scenarios like expression evaluation, recursion, and memory management.
