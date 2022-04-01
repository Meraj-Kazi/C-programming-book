## Chapter - 2. Conditionals / Decision Control

## Conditional Operator

Let's talk about a real life problem.

You have 1000 BDT in your wallet. And you need to buy something to eat. So, when you order something, the total price needs to be less than 1000. If your selected products are overpriced or total price is more than 1000, then you can not buy the items.

How can we do this through a simple computer program. The program will check if the total price is less than your balance or not! So, we will just write the condition we have said above and under the condition we will show the outputs. Let's see by example to make it more easier.

Example:
```c
int total_price;
scanf("%d",&total_price);
if(total_price > 1000) printf("You can't buy the item.\nIt is overpriced");
else printf("You can buy the item");
```
In the above example we have declared a variable `total_price` to store the total price of a item. Then we take the item price as input with `scanf()` funtion. After that, we have just checked the condition by `if(total_price > 1000)` and show the ouput under this condition,
<br>
```
You can't buy the item.
It is overpriced
```

Then, we will use `else`, if the condition `if(total_price > 1000)` is not satisfied and the total_price is less than or equal to your balance 1000 BDT. We will show output under the else condition,
<br>
```
You can buy the item.
```
Full Code:
```c
#include<stdio.h>
int main()
{
    int total_price;
    scanf("%d",&total_price);
    if(total_price > 1000) printf("You can't buy the item.\nIt is overpriced");
    else printf("You can buy the item");
    return 0;
}
```
We can do it in two more way. We can use two `if` condition without using the `if-else`. Or, we can also use `else if` instead of `else`. Let's see,<br><br>
Using Two `if` condition:
```c
#include<stdio.h>
int main()
{
    int total_price;
    scanf("%d",&total_price);
    if(total_price > 1000) printf("You can't buy the item.\nIt is overpriced");
    if(total_price <= 1000) printf("You can buy the item");
    return 0;
}
```
<br>Using `else-if`(It is also called else-if ladder):
```c
#include<stdio.h>
int main()
{
    int total_price;
    scanf("%d",&total_price);
    if(total_price > 1000) printf("You can't buy the item.\nIt is overpriced");
    else if(total_price <= 1000) printf("You can buy the item");
    return 0;
}
```
The `conditional` operator is also known as `ternary` operator which is represented by the symbols `?` and `:`. With this operator, we will check a condition if it is true or false and execute one statement between two. Simple `if-else` statement can be represented with this operator. Now We will directly go to the example of the conditional operator instead of getting bored by knowing it with theoretical description only.

Syntax:

```
(condition)? expression1 : expression2;
```

Example:

```c
int A = 200;
(A > 100)? printf("A is greater than 100"):printf("A is not greater than 100");
```

Here in the statement there is a condition `(A>100)`. We will use the `?` symbol to check the condition. If the condition is true then the expression before the `:` symbol will be executed otherwise the expression after the symble `:` will be executed. In the above example we assume `A=200`. So, the condition `(A>100)` is true and the expression

```c
printf("A is greater  than 100")
```

before the `:` symbol will be executed. We will see the line
`A is greater than 100` in the output terminal.<br>
Full code example:

```c
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
You can give any integer input -20, 19, 50, 101, 100, 205 or any whole number you want. If the condition is `true`, the output you will see,<br>
```
A is greater than 100
```
<br>Otherwise, the output you will see,<br>
```
A is not greater than 100
```
<br>
It is clear that the conditional operator always check the condition before the `?` symbol and if the condition is true then the expression before `:` symbol will be executed otherwise the expression after `:` symbol will be executed.<br><br>


### Problems For Practice

#### Problem Statement

Write a program with `if-else` condition to check the input number is odd or even.
Write a program with the `conditional operator` to check the input number is odd or even.
(result at result chapter in the end of this book)
