# Ex5 Stack Operations
## DATE:
## AIM:
To write a C function to perform push and pop operation of the stack in the infix to postfix conversion.

## Algorithm
1. Declare a stack array (stack[100]) and initialize top to -1 (empty stack).
2. Push operation (push(x)):
   Increment top and insert x into stack[top].
3. Pop operation (pop()):
   If stack is empty (top == -1), return -1 (error).
   Otherwise, return stack[top] and decrement top.
4. Stack follows LIFO (Last-In-First-Out) order.
5. Operations:
   push('A') → stack = ['A'], top = 0.
   pop() → returns 'A', stack = [], top = -1.

## Program:
```
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Jai Surya R
RegisterNumber:  212223230084

#include<stdio.h>

char stack[100];
int top = -1;

void push(char x)
{
    stack[++top] = x;
}

char pop()
{
    if(top == -1)
        return -1;
    else
        return stack[top--];
}
```

## Output:

![Screenshot 2025-04-29 200204](https://github.com/user-attachments/assets/f6df17ee-fe2c-4bd3-89e8-37dd76f8baf8)



## Result:
Thus the C program to perform push and pop operation of the stack in the infix to postfix conversion is implemented successfully.
