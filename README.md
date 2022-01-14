# Learn C Programming with Meraj Kazi 

A simple open source book to learn basics of C programming language easily. It'll help beginners to learn programming easily ^__^ 

It's totally free and written and maintained with ❤️ by our brilliant contributors. 

<br>

### Chapter List 

- [Chapter - 0. Before We Start](./chapters/chapter_0.md) 
- [Chapter - 1. Start Coding in C](./chapters/chapter_1.md) 
- [Chapter - 2. Conditionals / Decision Control](./chapters/chapter_2.md) 
- [Chapter - 3. Loop Control](./chapters/chapter_3.md) 
- [Chapter - 4. Case](./chapters/chapter_4.md) 
- [Chapter - 5. Functions](./chapters/chapter_5.md) 
- [Chapter - 6. Pointers](./chapters/chapter_6.md) 


## History in brief 
C language was originally developed by _Dennis Ritchie_ between 1969 and 1973 at Bell Labs. One of the most used programming language till today and still being used in numerous sectors of computer science.

 





## Conditional Operator
<br>The `conditional` operator is also known as `ternary` operator which is represented by the symbols `?` and `:`. With this operator, we will check a condition if it is true or false and execute one statement between two. Now We will directly go to the example of the conditional operator instead of getting bored by knowing it with theoretical description only.<br>
<br>Syntax:<br>
(condition)? expression1 : expression2;<br><br>
Example:<br>
```
int A = 200;
(A > 100)? printf("A is greater than 100"):printf("A is not greater than 100");
```
Here in the statement there is a condition `(A>100)`. We will use the `?` symbol to check the condition. If the condition is true then the expression before the `:` symbol will be executed otherwise the expression after the symble `:` will be executed. In the above example we assume `A=200`. So, the condition `(A>100)` is true and the expression
```
printf("A is greater  than 100")
```
before the `:` symbol will be executed. We will see the line 
`A is greater than 100` in the output terminal.<br>
Full code example:
```
#include<stdio.h>
int main()
{
    int A;
    printf("Enter a number to check if it is greater than 100: ");
    scanf("%d",&A);
    (A>100)? printf("A is greater than 100"):printf("A is not greater than 100");
    return 0;
}
```
Just compile and run it!<br>
You can give any integer input -20, 19, 50, 101, 100,  205 or any whole number you want. If the condition is `true`, the output you will see,<br>
`A is greater than 100`
<br>Otherwise, the output you will see,<br>
`A is not greater than 100`<br>
It is clear that the conditional operator always check the condition before the `?` symbol and if the condition is true then the expression before `:` symbol will be executed otherwise the expression after `:` symbol will be executed.<br><br>
### Problem : Write a program with the conditional operator to check the input number is odd or even. (result at result chapter in the end of this book)




## Functions