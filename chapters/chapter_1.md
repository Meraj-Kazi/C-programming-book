## Chapter - 1. Start Coding in C

(_From here, things get dirty_ :D ) <br>

First of all, I assume you're new to programming or new to C programming language. That's why you'll not understand many things at the beginning, but don't worry. Continue reading and keep going, you'll understand it all after some time. Sounds fair?! :p

**Let's begin then!**

Remember this portion of code as a frame for your basic learning. You need to use this code almost every time you write anything in C. It's like one of the base of C programming.

```
#include<stdio.h>

int main()
{


}
```

Seems like you're reading some alien language?! <br>
No, it's not like that :p <br>
After finishing the basics, you gonna love this portion of code for sure ^\_\_^

Now put this line of code between `{ }`

```
printf("Hello World!");
```

Your code should look like this:

```
#include<stdio.h>

int main()
{
    printf("Hello World!");

    return 0;
}
```

Now, coding part is done. We need to execute it. After executing we'll find out what this code does. <br>
To execute the code, look at the top border and click on the `Execute` button. A dropdown will come with some options. You'll click on `Comiple`. Then the code will be compiled. Compiling is checking if there's any mistake in the code. If there any, then it'll show that on the screen in down(CodeBlocs) or in another mini window(Dev C++). Our code has no bugs or mistakes, so there will be a message like `Successfully completed.......` or `Successfully compiled` etc. <br> <br>

Now we need to run this small program so that we can see what it does. So, click that `Execute` button once again and click on `Run`. <br>

### A black screen will come and there will be written `Hello World`. <br>

Now that we know our program is correct and we also know it prints a `Helllo World` on the screen, we can try to understand the code part by part.

## The meaning of `#include<stdio.h>`:

`stdio`= Standard Input Output. It is a header file which helps the computer to understand the codes in c. That's why we need to include it in the program at the very beginning. Without that header file, computer would not understand our code. As it's a header file, that's why it has a `.h` extension. <br>

## The meaning of `int main()`:

`int` means integer. Integer is a term in mathematics that refers to numbers without any decimal point. Example: 1,4,7,8 etc. are integers. `main()` is a function. Programming works as function. That means a computer program is nothing but a collection of one or more functions written in a programming language. So, for now, only thing that we need to remember is `int main()` is a function that helps us to build and run our programs in it. The programs written under any function has a `{` at starting point and a `}` at the end. So, it looks like this-

```
#include<stdio.h>

int main()
{


}
```

## The meaning of `printf("Hello World!");`:

`printf` is a inbuilt library function in C programming language which is available in C library by default. It is declared and related macros are defined in `stdio.h` which is a header file in C language. That's why we have to include `stdio.h` file as shown in the C program to make use of printf() library function in C language. <br>

Now, what does `printf` do ??? <br>
It displays everything on the screen which it has between it's `" "`. In this case we had 'Hello World!' written there. That's why it displayed 'Hello World!'. <br>

Let's try something else! Put name of your favorite person or place or anything else in the place of 'World' and see if it works. But you need to save it again by pressing `ctrl + s`, compile it and then run it. This is because, you made some changes in the code by replacing the word 'world' with another word. If we change even a comma(`,`) in the code, we need to save, compile again and then run it.

## The meaning of `return 0;`:

This program would run successfully without this line. Then the question remains <strong> "_Why did we put that then???_" </strong> <br>
Well, the answer is not that simple. For now, just keep it in mind that, `return 0;` indicates that the program performed successfully.

## _[_

### _Another important thing_

You may have noticed that we used a semicolon `;` after every line of our code. That's because it's mandatory. <br>
Now, why is it mndatory??? <br>
Well, the answer is pretty much simple! <br>
Compiler never thinks about spaces or line breakes. That means all the spaces or line breaks are never important for compiler. But if we don't keep any white space or line break, then the code would look like impossible to understand. <br>

This semicolon `;` indicates that the line ends at that point. <br>
That's why it is necessary to put a `;` after every line. <br>
And this piece of knowledge will always help you whenever you try to learn any new programming language.

## _]_

### And don't get bored seeing these as I'm moving slowly, because the more you understand these with you heart, the more you gonna rock in the next stage! <br>

Now then, let's move on to the next phage where we will learn to do some maths with programming using very much easy logics that student with poor knowledge of math can do. <br>
Let's try this code: <br>

```
#include<stdio.h>

int main()
{
    int a;
    a= 5;

    printf("value of a = %d", a);

    return 0;

}
```

Compile this code, run it and see the result. <br>
It displays `value of a = 5` <br>

In this line <br>

```
printf("value of a = %d", a);
```

The `%d` in the code gets the value of "a", which is written after the `",` symbols in the code. So, this line displays the number we saved in `a`. Couldn't we just write like this?- <br>

```
printf("value of a = a");
```

No, it wouldn't work. Because it would print "a" instead of printing the value of "a". To print the value, we need to put `%d` in between `" "` and write the variavble afer putting a comma(`,`) after it. But how about printing more than one numbers? <br>
Let's try this code! <br>

```
#include<stdio.h>

int main()
{
    int a,b;
    a= 5;
    b= 6;

    printf("a = %d and b = %d ", a, b);

    return 0;

}
```

Run this code. I hope you're seeing that first `%d` gets the value of first variable written after the comma(`,`). Second `%d` gets the value of second variable. That's how it works! Now find out if we declare a variable without storing any value in it, what will happen if we try to print it's value? <br>
Here's the code- <br>

```
#include<stdio.h>

int main()
{
    int a,b,c;
    a= 5;
    b= 6;

    printf("a = %d, b = %d and c = %d", a, b, c);

    return 0;

}
```

We declared three variables a, b and c. c had no value stored in it. So the result was something like 32766 or 32765 or any other odd number. This is known as garbage value. <br>

By the way, did you guys notice that we used `int a`, `int a,b` and `int a,b,c` in these codes?? <br>

## What's the meaning of this `int`?

Well, there are 3 kinds of data types. In simple language, we have 3 types of values.

### 1. Integer:

Integers are numbers without any decimal value. Example: 1, 4, 15, 2100 etc.
They're known as in `int` programming language.

### 2. Floating numbers:

Floating numbers or floats ar numbers with decimal point. Example: 2.5, 97.7 etc.
They're known as in `float` programming language.

### 3. Character:

They're alphabets. Example: a, d, e, A, M, S etc.
They're known as `char` in programming language. <br>

So, as we declared `int a`, that means it can only hold integer values. But what will happen if we try to put a floating value or value with decimal point in an integer variable? Let's see! <br>

```
#include<stdio.h>

int main()
{
    int a;
    a= 5.2;

    printf("a = %d", a);

    return 0;

}
```

What happens after running this code? <br>
you see something like this `a = 5` <br>

But we entered 5.2 in `a`. This happened because `a` is declared as int, that means it can only hold integer type value. As we entered a value with decimal point, it only took it's integer part and avoided the decimal point part.

Let's see this code again but with some additional things.

```
#include<stdio.h>

int main()
{
    int a;
    printf("Enter a number: \n");
    scanf(" %d", &a);

    printf("The number is: %d ", a);

    return 0;

}
```

Compile this code, run it and see the result. <br>

Another black screen comes in front of you and tells you to enter a number. If you enter a number, it displays the number you entered. <br>
Let's try to understand what's new in this code!!! <br>

First we declared an integer called `a`.
In the next line, the code was <br>

```
   printf("Enter a number: \n");
```

<br>

You already know about `printf` function, but `\n` is new for you. <br>
`\n` is an special symbol that gives a _line break_. That means, when I use `\n` in a line, that line finishes there.

## Meaning of `scanf(" %d", &a);`:

`scanf` is another library function which works as it is supposed to do, It's work is to get number from user. <br>
`%d` means it'll take an integer value from user. <br>
_[`%d` is for taking integer value, `%f` is for taking float values and `%c` is for char or characters]_ <br>

Now, because of `%d`, the function `scanf` will take a value from user, but where it'll store or save it???<br>
There comes the `&a`. We declared an integer variable `a` at the beginning of our program. We'll keep the value in `a`. To transfer the value from `%d` to `a` we use `&` symbol. So, `&a` puts the value in `a`. Now, remember, `a` is just a variable we declared at the beginning. We could name it anything. If we declared it as `int b` or `int random` or anything else, it would work just fine. Then we would have to use it like `&random`. Now, you've understood that, in `scanf(" %d", &a);`, user enters a value and `%d` receives it and sends it to `&a` <br> <br>

Then it displays the value with this line <br>

```
printf("The number is: %d ", a);
```

Now that we know about how C program works, let's dive deep! <br>

How can we do mathematical calculations in C? <br>
Look at this program: <br>

```
#include<stdio.h>

int main()
{
    int a,b,sum;
    printf("Enter two numbers to add: \n");
    scanf(" %d %d", &a, &b);

    sum = a+b;
    printf("The sum of those numbers is: %d", sum);

    return 0;

}
```

Compile and run it! <br>
Youe aee that, it prints the value of `sum` which is the result of adding `a` and `b`. Another thing we need to understand that we declared `sum` as a integer variable. How could we know that the result of adding `a` and `b` would be integer???<br>
Because, result of adding two integers is always an integer value and result of adding two floats is always a float value. That goes for other mathematical operations like division, multiuplication etc. too. Now, if you have understood this, then solve this problem below. <br>

### Problem : Write a program to add, subtract, multiply and divide two numbers input by user. (result at result chapter in the end of thus book)

<br><br><br><br>

### Modulus operator<br><br>

Now that we're knowing about C language little by little, we need to know something new. Let's talk about `modulus (%)` operator. <br>

Modulus operator helps us in many ways during programming. But before that, we need to understand what it actually does.
Let's see an example first, <br>

```
5 + 2 = 7
5 - 2 = 3

5 % 2 = 1

```

Looks weird?! <br>
In the example, 5 is divided by 2 and there remains a remainder 1. That is what modulus operator does. It gives us the remainder. <br>

Then guess the answers here: <br>

```
7   %  3   = ?
21  %  7   = ?
543 %  8   = ?
```

I think we understood the concept of <strong>Modulus</strong> operator pretty well enough.
Then let's move forward!
