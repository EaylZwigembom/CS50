#Artificial-Intelligence
Let's say you were trying to implement a **chatbot**, for instance, that just **==answers questions and has conversations with you==**.

You can do that using [[Pseudocode]] and as we'll soon see, you could do that also using **programming languages** like Python, C, and other languages...

But **pseudocode** might look like this when implementing a **chatbot**:

```
If student says hello
	Say hello
Else if the student says goodbye
	say goodbye
Else if the student asks how you are
	say well
```

But, if we make a **chatbot** in that way, that means we will have to **program** a scenario for **==every question possible==** the user can ask. So does that mean we will program a scenario like this?

```
...
Else if student asks you why 111 in binary is 7 in decimal
```

Notice how just to program a **handful** of interactions, 
**many lines of code would be required**. How many lines of code would be required for thousands or tens of thousands of **==possible interactions==**?

Rather than programming conversational AI like the above, AI programmers train ==**_large language models_ (LLMs**)== on large datasets.

 **LLMs** look at patterns in **large blocks** of language. Such language models attempt to create a ==**best guess**== of what words come after one another or alongside one another.

 ![[Pasted image 20250617191241.png]]

**LLMs** are typically implemented with what is called: **==Neural Networks==**. 
And what computer scientist have been doing is implementing a software using literally **`0`**'s and **`1`**'s, graphs or **neural networks** that might look like the picture above, where each circle represents a **==neuron==** and each arrow represents a **==pathway==** between them, and provides **==inputs==** huge amounts of **data** into these networks, and what these **LLMs** do in the process is use **statistics** and **probability** and try to **output** the most probabilistically likely answer to the **input**.

---

CS50’s own AI-based software tool called [CS50.ai](https://cs50.ai/) is an AI helper that you can use during this course. It will help you, but not give away the entire answers to the course’s problems.
You are not permitted to use any AI in this course except the [CS50.ai](https://cs50.ai/)
