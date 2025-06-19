#Binary

**Binary**, also known as the ==**binary system**== or **`base-2`** 
==**is the way computers can understand and process data==**. 


##### **Binary Digits (Bits)**
^bits

The ==**binary system**== is made out of series of ==**binary digits** **(bits)**==.
each **==bit==** can be represented as ==**0**== or ==**1**==.

But how can we compare this information to information from the real world? Because in the real world we don't just use **`0`** and **`1`**, we use **`0`** to `9`. 

Let's say you have **3 bits** **(3 different possibilities of 0 and 1)**. The first thought will be that you can count tup to 3 and that's it. But you can be more clever by **representing each number as one of the different possibilities 3 bits have**, because again each **bit** can be **0** or **1**. 

If you know math you will know that **3 bits** will have **8 different possibilities**: **$2^3 = 8$**. 
==**2**== is for each possibility in a bit **(0 or 1)** and ==**3**== is for the **3 bits** you have.
This is also known as ==**base-2 (2 to the power of n)**==.

If you use that you can count up to high as **`7`** **(because you start from `0`)**:

**`0`** will be represented as: **`000`**
**`1`** will be represented as: **`001`**
**`2`** will be represented as: **`010`**
**`3`** will be represented as: **`011`**
**`4`** will be represented as: **`100`**
**`5`** will be represented as: **`101`**
**`6`** will be represented as: **`110`**
and **`7`** will be represented as: **`111`**

Well how are these patterns of **`1`** and **`0`** are created and what is it that our computers are actually doing?

Well, it's actually doing something a little like how we count ourselves

In the real world we use the [base-10/decimal](https://www.google.com/search?q=base-10&sxsrf=AE3TifMB3O0a5babxdBAu2dI5gNKiZgXJg%3A1750050301236) counting method

![[Pasted image 20250616075419.png]]
This image for example shows the ==number one-hundred twenty three==.
But why is that exactly that number?

![[Pasted image 20250616075431.png]]
Well if you were in grade school, you were taught that there are **columns** of numbers **(1, 10, 100, ...)** and each number in that column ==**represents itself times the number that column stands for**==. 
for example if we put the number **2** in the column of **100** we would get **200**: **2 * 100 = 200**.

![[Pasted image 20250616075443.png]]
You can also see that each **column** is **==10 to the power of n==**. that's why this method of counting is called ==**base-10**==. **each column has 10 different possibilities (0 through 9).**

![[Pasted image 20250616075453.png]]
But in the **binary world** computers only have **0** and **1** because all they have physically are **transistors**. Tiny light bulbs that can be **off** or **on** 
**(0 for off, 1 for on).** And if you have only **==2 digits==** to play with, the **base-10** should turn into **base-2** **==(2 different possibilities for each column).==**

![[Pasted image 20250616075507.png]]
And now, if we do the math we get the column of 1s column, the 2's column, the 4's column, and so on (As seen in the picture above). 
And now if we take a look again at the **number representation of 3 bits** we can start seeing why it all makes sense:

**0** will be represented as: ==**000**==: $0 * 1 + 0 * 2 + 0 * 4 = 0$
**1** will be represented as: ==**001**==: $1 * 1 + 0 * 2 + 0 * 4 = 1$
**2** will be represented as: ==**010**==: $0 * 1 + 1 * 2 + 0 * 4 = 2$
**3** will be represented as: ==**011**==: $1 * 1 + 1 * 2 + 0 * 4 = 3$
**4** will be represented as: ==**100**==: $0 * 1 + 0 * 2 + 1 * 4 = 4$
**5** will be represented as: ==**101**==: $1 * 1 + 0 * 2 + 1 * 4 = 5$
**6** will be represented as: ==**110**==: $0 * 1 + 1 * 2 + 1 * 4 = 6$
and **7** will be represented as: ==**111**==: $1 * 1 + 1 * 2 + 1 * 4 = 7$

And how a might a computer count up to **8** if **3 bits** can only count to **7**?

The computer will add another bit and it's column will be an **==8 column==**, because the first 3 columns were:

**$2^0 = 1$**
**$2^1 = 2$**
**$2^2 = 4$**
and next is $2^3$ which is **8**.
so the number **8** would be displayed as: **==1000==**.

And how will computers with excel or any kind of other number crunching software count really high and keep track with really big numbers? 
The computer will just throw more and more bits at the software until it can represent the number that is needed.

But 1 bit, 3 bits, even 4 bits aren't that useful because we have to deal with numbers like 35 or 256. And that's why we have bytes.

##### **Bytes**
^bytes

Byte is a series of **==8 bits==**. 

![[Pasted image 20250616093946.png]]
This is how a byte looks like in binary code. And the biggest number **==1 byte==** can represent is **==256==**: 
$1 *128 + 1 * 64 + 1 * 32 + 1 * 16 + 1 * 8 + 1 * 4 + 1 * 2 + 1 * 1 = 255$
Then you add the **absolute** **0** and you get **==256==**.

0