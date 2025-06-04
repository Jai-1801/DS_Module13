# Ex4 Evaluation of prefix expression
## AIM:
To write a C function to evaluate the given prefix expression using stack and print the output of the given prefix expression from the stack inside the function . 

## Algorithm
1.Initialize a stack (s[]) and a top pointer (top = 0).

2. Scan the prefix expression from right to left:
   If the character is an operand, push it onto the stack.
   If the character is an operator (- or *), pop the top two elements, apply the operation, and push the result back.
   
3. Repeat until the entire expression is processed.
  
4. The final result will be the only remaining element in the stack.
  
5. Print the result and exit.

## Program:
```
Program to evaluate the given prefix expression
Developed by: Jai Surya R
RegisterNumber:  212223230084

 int s[50];
int top=0;

void push(int ch)
{
	top++;
	s[top]=ch;
}

int pop()
{
	int ch;
	ch=s[top];
	top=top-1;
	return(ch);
}

void evalprefix(char p[50])
{

    int a,b,c,i;
    for(i=strlen(p)-1;i>=0;i--)
	{
		
		if(p[i]=='-')
		{
		a=pop();
		b=pop();
		c=a-b;
		push(c);
		}
		else if(p[i]=='*')
		{
		a=pop();
		b=pop();
		c=a*b;
		push(c);
		}
	   else
		{
			push(p[i]-48);
		}
			
	}
	printf("%d",pop());
}
```

## Output:

![Screenshot 2025-04-29 195700](https://github.com/user-attachments/assets/3e3d2fb1-4543-41d9-8d45-f27f39839daf)





## Result:
Thus, the C program to evaluate the prefix expression using stack and print the output of the given prefix expression from the stack inside the function is implemented successfully.
