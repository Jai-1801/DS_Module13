# EX 1 Display operator precedence in the infix expression.
## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1.Start the program.
2.Read the postfix expression from the user.
3.Traverse each character in the expression.
4.If the character is an operator, determine its precedence.
5.Display the operator and its precedence.
6.End the program.   

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Jai Surya
RegisterNumber: 212223230084
*/

#include <stdio.h>
#include<string.h>

int main()
{
   int i,j;
   char ch[100];
   strcpy(ch,"(A*B)^C+(D%H)/F&G");
   for(i=0;ch[i]!='\0';i++)
   {
       j =ch[i];
       switch(j)
       {
           case '*':
           {
               printf("%c  ----> Second Highest Priority\n",ch[i]);
               break;
           }
           case '^':
           {
               printf("%c  ----> Highest Priority\n",ch[i]);
               break;
           }
           case '+':
           {
               printf("%c  ----> Second Lowest Priority\n",ch[i]);
               break;
           }
           case '%':
           {
               printf("%c  ----> Second Highest Priority\n",ch[i]);
               break;
           }
           case '/':
           {
               printf("%c  ----> Second Highest Priority\n",ch[i]);
               break;
           }
           case '&':
           {
               printf("%c  ----> Lowest Priority\n",ch[i]);
               break;
           }
       }
   }
   

   
    return 0;
   
}
   
```

## Output:
![image](https://github.com/user-attachments/assets/51555b1f-6868-4dbd-acec-8d93f288b7f3)



## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
