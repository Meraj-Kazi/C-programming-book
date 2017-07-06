<link href="css/style.css" rel="stylesheet">

# Learn C Programming 
## with Meraj Kazi

A simple book to learn basics of C programming language easily. It'll help beginners to learn programming easily ^__^ 

<br><br><br>

## History in brief 
C language was originally developed by _Dennis Ritchie_ between 1969 and 1973 at Bell Labs. One of the most used programming language till today and still being used in numerous sectors of computer science.

## Before we start:
We need a compiler software installed in our PC in which we'll write, compile and run our codes in C. 
Here's is a list of some C language compilers:

- [Codeblocks](http://www.codeblocks.org/downloads/26)
- [Dev C++](https://sourceforge.net/projects/orwelldevcpp/) 
- [Vim](http://www.vim.org/download.php) (_my favourite, but don't try if you're a biginner_) 
- Turbo C etc.

Codeblocks or Dev C++ will be better choice for beginners. So, download any one of those and install it in your PC. After installing successfully, open it. Go to the top left and click on the tab named `File` and select `new file` or `new source file` or just `new` and then `source file`. 

![New source file](img/NewSourceFile.jpg)


Then you'll get a blank file opened in front of you. First, you need to save it as C file format because right now it is just a text file with no format. To make it a C file you need to save it in C format. To save it in C format, click on that top left `File` again and click on `save as` and then a new window will come.<br><br><br> 
Look at the downside of that new window. You'll see the filename and format. Delete all and name it **_test.c_**. Here `.c` is the format and **_test_** is the name. You can give it another name but format must be `.c`. <br><br> 
And there should be **_no blank space_** in name. Suppose, file names like `my first program` is not valid. It should be like `my-first-program.c` or `MyFirstProgram.c`. Whatever you put as name, there shoud be `.c` after the name because that defines the format of C language. 



## Start Coding in C
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
After finishing the basics, you gonna love this portion of code for sure ^__^

Now put this line of code between `{  }` 

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
A black screen will come and there will be written `Hello World`. <br> 

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

Let's try something else! Put name of your favorite person or place or anything else in the place of 'World' and see if it works. But you need to save it again by pressing `ctrl + s`, compile it and then run it. This is because, you made some changes in the code by replacing the word 'world' with another word. If we change even a `,` in the code, we need to save, compile again and then run it.

## The meaning of `return 0;`:
This program would run successfully without this line. Then the question remains <strong> "_Why did we put that then???_" </strong> <br>
Well, the answer is not that simple. For now, just keep it in mind that, `return 0;` indicates that the program performed successfully.

### _Another important thing_
You may have noticed that we used a semicolon `;` after every line of our code. That's because it's mandatory. <br>
Now, why is it mndatory??? <br>
Well, the answer is pretty much simple! <br>
Compiler never thinks about spaces or line breakes. That means all the spaces or line breaks are never important for compiler. But if we don't keep any white space or line break, then the code would look like impossible to understand. <br>

The `;` indicates that the line ends at that point. That's why it is necessary to put a `;` after every line.
