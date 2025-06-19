#C #Compiling


![[Pasted image 20250619160349.png]]
**Compiling** is the **==process of taking your input which is the ==**
**==source code(C, Java, Swift, etc...) and turning it into what's called 
machine code==** ([[Binary]]). The **compiler** is an **algorithm**([[Algorithms]]), embodied in a **program** that we can run. But how do we actually get from source code to machine code?

Well, up until now, when you want to **compile** a program
(Let's say the name of the program will be: **hello**).

You write:
```
make hello
./hello
```

which is a bit weird, but **make** **hello** says: **==compile the program called hello==**
and **./hello** says: **==run the program called hello in the current folder==**. This command is equivalent to double clicking an icon of an app in your desktop.

But the command "**make**" is **not** actually a compiler. It is a **program**, a very helpful program, but it **==automates the process of running an actual compiler for you==**.

```
clang hello.c
./a.out
```
There's **many** different compilers in the world but the one we will use in this class is free, and open-source, and therefor very popular in the world, is actually called: **==clang (For: C Language)==**. And so really what's happening when you run **make hello** or any other such command in turn is running another program for you called **==clang==**. 
The catch though is that this program by default **==is not nearly as user friendly==**. and it doesn't even give you a useful input. By default the program that the clang gives you is called **a.out**. which is stands for **Assembly Output**. So how can we make the name of the program make more sense? 

Well we can use what's called 
[[Command Line Arguments]]. In **clang** we can do this by instead of just typing clang, and the name of the source code, we can add an **==argument==** before the name of the program to change the name:

```
clang -o hello hello.c
./hello
```
So you see that there is this **==-o==** in the program and this thing is called a 
**flag or a switch**(Whichever you would like to call it), which is basically an **argument** that helps you modify the command. This command says: **==Output(From here comes -o) a file named hello when you compile hello.c. ==**

```
clang -o hello hello.c -lcs50
./hello
```