#Color

In every screen there are **pixels**. Each **pixel** has **`3` microscopic LEDs** Each **LED** is showing a color out of the **`3`** main colors that make the rest of the colors: **==Red, green, and blue==**. Here is a picture of **pixels** under a microscope, `1` pixel is `3` LEDs: Red, green, and blue:

![[Pasted image 20250616145945.png]]

**But how do the computers know what color to display? And how can they turn literally `0`'s and `1`'s into colors?**

#### **RGB**
**RGB(Red, Green, Blue)**, is ==**a system that computers use to turn binary numbers into color**==. Each color in **RGB**: **Red, Green, Blue** is represented by a **byte**([[Binary#^Bytes]]). that means that the **value** of each color is 
between **`0`** and **`255`** **(In total there are `3` bytes: `24` bits per pixel)**. 
That way, by playing with the numbers you can get any **color** you want.