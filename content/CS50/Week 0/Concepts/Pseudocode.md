#Pseudocode

**Pseudocode** is **==a process of converting instructions into code==**.
The ability to create pseudocode is **central** to one's success in CS50 and in computer programming. It is **not** a formal language, therefor there are many correct ways to write pseudocode

**Pseudocode** is **==a human-readable version of your code==**, and is used to gain a deeper understanding of the **problem** and the **logic** you use to **solve** it. For example, considering the third algorithm([[Algorithms]]) from the 
**phone book** example ([[Algorithms#^Phone-Book]]), we could create pseudocode like this:

```
1  Pick up phone book
2  Open the middle of phone book
3  Look at page
4  If person is on page
5       Call person
6  Else if person is earlier in book
7       Open middle of left half of book
8       Go back to line 3
9  Else if person is later in the book
10      Open middle of right half of book
11      Go back to line 3
12  Else
13      Quit
```

###### **Pseudocoding is such an important skill for at least two reasons:**

- First, when you *pseudocode* **before** you create formal code, it allows you to **==think through the logic of your problem==** in advance and it will make you able to create the **formal code** in a more **efficient** way. 

- Second, when you pseudocode, you can later **==provide this information==** to others that are seeking to **understand** your coding decisions and how your code works.

###### **Notice that the language within our pseudocode has some unique features.** 

- First, some of these lines begin with verbs like **pick up**, **look at**. Later we will call these **==functions==**.

- Second, notice that some lines include statements like **if** or **else if**. These are called **==conditionals==**.

- Third, notice how there are expressions that can be stated as **true** or **false**, such as "**person is earlier in the book**". We call these **==boolean expressions==**.

- Finally, notice how there are statements like "**Go back to line 3**". These we call **==loops==**.

  ==**These building blocks are the fundamentals of programming**==.
---
