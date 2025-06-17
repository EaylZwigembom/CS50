
([[Computer Science#^Problem-Solving]])
#### **What Is An Algorithm?**

An **algorithm** is a **==step-by-step==** **set of instructions to solve a problem**.
A computer is a **dumb machine**, and because of that, the **algorithm** has to be very **precise** so the computer will be able to perform it and give the **==output==** that you wanted.

There are many **different** ways to make an **algorithm** to solve your **==problem/input==**. But the question is: **which of these ways that I solve the problem is the fastest, and most efficient?**

##### **For Example:**

Let's say we want to locate a **single name** in a phone book, for this example's sake the name will be **John Harvard**.

One approach could be going through **==every single==** page in the book until you find **John Harvard**

Another approach could be searching **==two pages at a time==**

A final perhaps better approach could be **==go to the middle of the phone book==** 
and ask, **"Is the name John Harvard to the left or to the right?"** Then, **==repeat==** this process, cutting the problem in half and half and half.

These are examples of **3 different** **algorithms** solving **the same problem**, some **efficient**, some **less efficient**. The **speed** of **each** of these **algorithms** can be pictured as in what is called 
**==big-O notation==**. but before we'll see the **big-O notations** of each of these algorithms,
we need to **understand** what a **big-O notation** is.

#### **big-O Notation**

##### **What is a big-O notation?**
a big-O notation is a way to determine **how the time it takes to the algorithm to solve the problem increases as the size of the 
==input/problem== ([[Computer Science#^Problem-Solving]]) increases**. 

Examples of big-O notations

| Big-O    | Name          | Explanation                                                                                                                                      | Example                                                                                                                                                                                                                                      |
| -------- | ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O(1)     | Constant time | No matter what, the runtime of the algorithm will always do the same amount of work                                                              | Let's say in a gym has **100** locker and your locker **54**, the next week the gym adds **100** **more** lockers, even though the **problem size was doubled**, you still go to locker **54**. **and It will take the same amount of time** |
| O(log n) | Logarithmic   | Cut the problem size by a **constant** number **every step**. For Example: Total steps = log₂(n). (log base-2).<br><br>Used in **Binary-Search** | log₂(n) as we saw in the phone book **algorithm** that **cuts** the **problem** in **half** until it finds the name **Jhon Harvard**                                                                                                         |

---

 **Now, let's get back to our phone book example and see how it works beneath the hood:**

![[Pasted image 20250616164459.png]]

 Notice that the **first algorithm** (Going through every single page), 
 highlighted in **red**, has a **==big-O==** of **`n`** it would take up to **100** tries to find the **correct name**. 
 
 The **second algorithm** (Going through two pages at once) has a **big-O** of **`n/2`** 
 it would take up to **50** tries to find the **correct name**. 
 
 The final and the **fastest algorithm** has a **big-O** of **`log2n`**, and you can see how slow the **big-O (Time to solve)** grows, Let's say again we have **100** names.
 So because we **==cut in half==** the **==problem/input==**([[Computer Science#^Problem-Solving]]) 
 **every try** until we find the **correct name**, it would take up to roughly **10** tries to find the **correct name**.


**==NOTE:==** The graph doesn't images the actual runtime of an algorithm but it images: 
**runtime** vs **problem size**.

##### here is a table that compares the graphs big-Os:

| **Big-O()**    | **Size Of Problem** | **Amount Of Tries**          |
| -------------- | ------------------- | ---------------------------- |
| **`O(n)`**     | **`100`** names     | up to **`100`** tries        |
| **`O(n/2)`**   | **`100`** names     | up to **`50`** tries         |
| **`O(log2n)`** | **`100`** names     | up to roughly **`10`** tries |

---
##### **How It Works In Math**

Let's say we have 100 pages in the phone book:

**`big-O(n)`** = **`1 * 100`** tries. because we go through every page in the phone book meaning for every page (n) there is 1 try.
 
**`big-O(n/2)`** = **`100/2 = 50`** tries. Because we go through 2 pages each time, meaning for every 2 pages in the phone book. we have 1 try. It works also if we go through 4 pages(for this algorithm it won't work because of the model, this example is just for understanding the concept) it will be: big-O(n/4) = 100/4 = 25 tries. meaning for every 4 pages we have 1 try.

**`big-O(log2n)`** = **`log2(100) = roughly 10`** tries. Because we cut the problem size (number of pages) in half every try until there is only one page left. meaning for every try the problem size is cut in half. This also works for cutting the problem size in 4 (for this algorithm it won't work because of the model, this example is just for understanding the concept) meaning: big-O(log4n) = log4(100) = around 60 tries.


---
