# EX3 Implementation of Tower of Hanoi
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm

1.Start the program.
2.Define the recursive function TOH(n, x, y, z).
3.If n > 0, call TOH(n-1, x, z, y).
4.Print the move from rod x to rod y.
5.Call TOH(n-1, z, y, x).
6.Call the function from main() with n = 4.
7.End the program.


## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: Jai Surya R
RegisterNumber: 212223230084
*/

#include <stdio.h>

void TOH(int n, char x, char y, char z)
{
    if (n > 0)
    {
        TOH(n - 1, x, z, y);
        printf("%c to %c\n", x, y);
        TOH(n - 1, z, y, x);
        return;
    }
}

int main()
{
    int n = 4;
    TOH(n, 'A', 'B', 'C');
    return 0;
}

```

## Output:
![image](https://github.com/user-attachments/assets/92938c30-7635-464d-90a7-df53cd5ea172)




## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
