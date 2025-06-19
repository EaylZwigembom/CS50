#Algorithms
([[Computer Science#^Problem-Solving]])
#### **What Is An Algorithm?**

An **algorithm** is a **==step-by-step==** **set of instructions to solve a problem**.
A computer is a **dumb machine**, and because of that, the **algorithm** has to be very **precise** so the computer will be able to perform it and give the **==output==** that you wanted.

There are many **different** ways to make an **algorithm** to solve your **==problem/input==**. But the question is: **which of these ways that I solve the problem is the fastest, and most efficient?**
The **speed** of **each** of an **algorithm** can be pictured as in what is called 
**==big-O notation==**


---
#### **Big-O Notation**

##### **What Is A Big-O Notation?**
a big-O notation is a way to determine **how the time it takes to the algorithm to solve the problem increases as the size of the 
==input/problem== increases**. 

##### **Examples Of Big-O Notations**

| Big-O    | Name          | Explanation                                                                                                                                      | Example                                                                                                                                                                                                                                      |
| -------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O(1)     | Constant time | No matter what, the runtime of the algorithm will always do the same amount of work                                                              | Let's say in a gym has **100** locker and your locker **54**, the next week the gym adds **100** **more** lockers, even though the **problem size was doubled**, you still go to locker **54**. **and It will take the same amount of time** |
| O(log n) | Logarithmic   | Cut the problem size by a **constant** number **every step**. For Example: Total steps = log₂(n). (log base-2).<br><br>Used in **Binary-Search** | log₂(n) as we saw in the phone book **algorithm** that **cuts** the **problem** in **half** until it finds the name **Jhon Harvard**                                                                                                         |
##### **Big-O Notation Graph**
**![](https://lh7-rt.googleusercontent.com/slidesz/AGV_vUfZpWEFUjgYPtoeX1tet6HAqrwkFUaNv_LZ1v-uhmPMvoq0VCukYlslAOImRqayYVHEjhSfPaW-K7SY3GjztlIxsmf52jS6XXo4L7A0FpYe8bs9d0wTtOKerpE0uBVqq7So6AnDT38jpcu35P-EE96pckCTDJPn=s2048?key=13zS9y-MjjTHuAQkELahQA)
 This is a big-O notation graph, you can see that the X axis is representing the size of the problem/input, and the Y axis is representing the time it takes to solve that problem.
 
 **`X`** axis: **Size of problem**
 
 **`Y`** axis: **Time to solve**

---
 

#### **The Phone Book Example:**

^Phone-Book

Let's say we want to locate a **single name** in a phone book, for this example's sake the name will be **John Harvard**. Let's say the book has **`1000`** pages.

One approach could be going through **==every single==** page in the book until you find **John Harvard**

Another approach could be searching **==two pages at a time==**

A final perhaps better approach could be **==go to the middle of the phone book==** 
and ask, **"Is the name John Harvard to the left or to the right?"** Then, **==repeat==** this process, cutting the problem in half and half and half.

These are examples of **`3` different** **algorithms** solving **the same problem**, some **efficient**, some **less efficient**. Now, let's see the big-O notation of each of these algorithms

![[Pasted image 20250616164459.png]]

 Notice that the **first algorithm** (Going through every single page), 
 highlighted in **red**, has a **==big-O==** of **`n`** it would take up to **1000** tries to find the **correct name**. 
 
 The **second algorithm** (Going through two pages at once) has a **big-O** of **`n/2`** 
 it would take up to **500** tries to find the **correct name**. 
 
 The final and the **fastest algorithm** has a **big-O** of **`log2n`**, and you can see how slow the **big-O (Time to solve)** grows, Let's say again we have **1000** names. So because we **cut in half** the **==problem/input==** **every try** until we find the **correct name**, it would take up to roughly **10** tries to find the **correct name**.


**==NOTE:==** The graph doesn't images the actual runtime of an algorithm but it images: 
**runtime** vs **problem size**.
###### here is a table that compares the graphs big-Os:

| **Big-O()**    | **Size Of Problem** | **Amount Of Tries**          |
| -------------- | ------------------- | ---------------------------- |
| **`O(n)`**     | **`1000`** names    | up to **`1000`** tries       |
| **`O(n/2)`**   | **`1000`** names    | up to **`500`** tries        |
| **`O(log2n)`** | **`1000`** names    | up to roughly **`10`** tries |

---
##### **How It Works In Math**

**`big-O(n)`** = **`1 * 1000`** tries. because for **every** page (**`n`**) in the book, the algorithm is doing **`1`** try.
 
**`big-O(n/2)`** = **`1000/2 = 50`** tries. Because we go through **`2`** pages every **`1`** try. 

**`big-O(log2n)`** = **`log2(1000)` = roughly `10`** tries. Because we cut the 
problem size (number of pages) in half **every** try until there is only **`1`** page left. 

---

When it comes to implementing algorithms as programmers, we taek the algorithms that maybe were aexpressed in English or any other human language and implement them into code using programming languages such as: C, C++, Python, R, Ruby, etc...
But how can we make sure our algorithms are efficient and don't do unessecary stuff? Because reading line after line of code in your algorithm may be not the best option and will just result you in an headace. So that's why we have [[Pseudocode]].