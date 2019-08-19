# **Exercise: For Loop**

1. Sum Numbers

Write a program that reads **n integers** and finds their **sum**

- On the first line of input read the **count** of numbers **n**
- Of the next **n** lines one introduces a whole number

The program should read the numbers, sum them and print the sum on the console.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | 30 | | 3 | -60 | | 4 | 43 | | 1 | 999 | | 0 | 0 |
| 10 | | | -10 | | | 45 | || 999 | | | | | | | |
| 20 | | | -20 | | | -20 | ||  | | | | | | | |
| | | | -30 | | | 7 | | | | || | | | | |
| | | | | || 11 | | | | | | | || | | |


2. Number sequence

Write a program that reads the **number of n integers**. Print out the **largest** and **smallest** number among the entered.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 5 | Max number: 304 | | 6 | Max number: 1000 |
| 10 | Min number: 0 | | 250 | Min number: 0 | |
| 20 | | | 5 | | 
| 304 | | | 2 | | 
| 0 | | | 0 | | 
| 50 | | | 100 | | 
| | | | 1000 | | 


3. Numbers Ending in 7

Write a program that prints the numbers in the **range [1 ... 1000], which ends in 7**.

| **Input** | **Output** |
| --- | --- |
| (no input) | 7 |
| | 17 |
| | 27 |
| | ... |
| | 997 |


4. Vowels Sum

To write a program that reads **text (string)**, entered by the user, **calculates** and **prints** the **sum** of the **values** of the **vowel** letters according to the table below:

| letter | a | e | i | o | u |
| --- | --- | --- | --- | --- | --- |
| value | 1 | 2 | 3 | 4 | 5 |

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| hello | 6 | e + o = 2 + 4 = 6 |
| hi | 3 | i = 3 |
| bamboo | 9 | a + o + o = 1 + 4 + 4 = 9 |
| beer | 4 | e + e = 2 + 2 = 4 |


5. Odd / Even Position

Write a program that reads the **n** - **count** of **numbers** entered by the user, and **calculate** the **amount** of the **minimum** and **maximum** numbers of **odd** and **even** positions (counting from **1** ). If there **is not** minimum/maximum element print **&quot;No&quot;**.

The output to be **formatted** in the following form:

**&quot;OddSum = &quot;** + {**sum** of the numbers on **odd** positions},

**&quot;OddMin = &quot;** + {**minimum** value of the numbers of **odd** positions } / {**&quot;No&quot;**},

**&quot;OddMax = &quot;** + {**maximum** value of the numbers of **odd** positions } / {**&quot;No&quot;**},

**&quot;EvenSum = &quot;** + {**sum** of the numbers of **even** positions },

**&quot;EvenMin = &quot;** + {**minimum** value of the numbers of **even** positions } / {**&quot;No&quot;**},

**&quot;EvenMax = &quot;** + {**maximum** value of the numbers of **even** positions } / {**&quot;No&quot;**}

**Each number should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 5 | OddSum=8.00, | | 0 | OddSum=0.00, |
| **3** | OddMin=-3.00, | | | OddMin=No, |
| -2 | OddMax=8.00, | | | OddMax=No, |
| **8** | EvenSum=9.00, | | | EvenSum=0.00, |
| 11 | EvenMin=-2.00, | | | EvenMin=No, |
| **-3** | EvenMax=11.00 | | | EvenMax=No |


6. Equal Pairs

There are **2 \* n**** -**the count** of numbers. The first and second form a **pair**, the third and fourth also, etc. Each pair has **value** - the **sum** of the component numbers. Write a program that checks **whether all couples have equal value**. Otherwise prints **the maximum difference** between **two consecutive** couples. If all couples have **equal** value, print **&quot;Yes, value = {value}&quot; + value**. Otherwise, print **&quot;No, maxdiff = {difference}&quot; + the maximum difference**.

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 3| Yes, value=3 | values = {3, 3, 3}|
| 1| | equal values|
| 2| | |
| 0| | |
| 3| | |
| 4| | |
| -1| | |



| **Input** | **Output** | **Comment** |
| --- | --- | --- |
| 4| No, maxdiff=4 | values = {2, 4, 4, 0}|
| 1| | differences = {2, 0, 4}|
| 1| | max difference = 4|
| 3| | |
| 1| | |
| 2| | |
| 2| | |
| 0| | |
| 0| | |


7. Grades

Write a program to **calculate statistics** of the exam **grades**. In the beginning, the program receives the **number** of **students** attended the examination and **its grade for each student**. In the end, the program should print **the percentage of students** with grade between **2.00 and 2.99**, between **3.00 and 3.99**, **4.00 and 4.99**, and between **5.00 or more**. Also the **average grade** of the exam.

### **Input**

Read from the console a **series of numbers**, each on a **separate** line:

- The **first** line - **number** of students **attended** the exam - **an integer in the range [1 .. 1000]**
- **For each student on a separate line** - **grade of the exam - real number in the range [2.00 ... 6.00]**

### **Output**

**Print** on the console **5 rows** that contain the following information:

First line - **&quot;Top students: {percent student with grade 5.00 or more}%&quot;**

Second line - **&quot;Between 4.00 and 4.99: {between 4.00 and 4.99 inclusive}%&quot;**

Third line - **&quot;Between 3.00 and 3.99: {between 3.00 and 3.99 inclusive}%&quot;**

Fourth line - **&quot;Fail: {less than 3.00}%&quot;**

Fifth line - **&quot;Average: {average grade}&quot;**

All numbers must be **formatted** to the **second decimal place**.

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 10 | Top students: 30.00% | Students with grade 5 and more – three = 30% of 10 |
| 3.00| Between 4.00 and 4.99: 30.00% | Between 4 and 4.99 – three = 30% of 10|
| 2.99| Between 3.00 and 3.99: 20.00% | Between 3 and 3.99 – two = 20% of 10|
| 5.68| Fail: 20.00% | Less than 3 – two = 20% of 10|
| 3.01| Average: 4.06 | Average grade: 3 + 2.99 + 5.68 + 3.01 + 4 + 4 + 6 + 4.50 + 2.44 + 5 = 40.62 / 10 = 4.062|
| 4| | |
| 4| | |
| 6.00| | |
| 4.50| | |
| 2.44| | |
| 5| | |



| **Input** | **Output** |
| --- | --- |
| 6 | Top students: 33.33% |
| 2| Between 4.00 and 4.99: 16.67% | |
| 3| Between 3.00 and 3.99: 16.67% |
| 4| Fail: 33.33% |
| 5| Average: 3.70 |
| 6| |
| 2.2| |

# Examples for Exam Problems

8. \* Clever Lily

Lily is now **n** years old. For every **birthday** she received a gift. For **odd** birthdays (**1, 3, 5 ... n**) she gets **toys**, and for each an **even** (**2, 4, 6, ... n**) gets **money**. For the **second** birthday gets **10.00$, the sum shall be increased by 10.00$ for each next even birthday (2 -> 10, 4 -> 20, 6 -> 30, etc.)**. Over the years, Lilly secretly been saving money. Lily&#39;s **brother**, in the **years** that she **gets money, taking on 1.00$ from them**. Lilly **sold the toys** received over the years, **each for P$** and **add** the amount to the **saved money**. With the money she wanted to buy a **laundry for X$**. Write a program that **calculates how much money was collected** and **whether it had enough to buy a washing machine**.

### **Input**

The input consist of **3** numbers entered by user, **each** on a **separate** line:

- **Lily&#39;s age** - **an integer in range [1...77]**
- **The laundry&#39;s price** - **floating-point number in range [1.00...10 000.00]**
- **Price per toy** - **an integer in range [0...40]**

### **Output**

Print on the console a **single line:**

- If Lily&#39;s money **are enough**:
  - **&quot;Yes! {N}&quot;** - where **N** is the rest of the money after purchase
- If the money **are NOT enough**:
  - **&quot;No! {М}&quot;** -  Lily needs **M** money more
- The numbers **N and M must for formatted to the second decimal place**.

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 10 | Yes! 5.00 | First birthday gets a toy; **2nd -> 10$**; 3rd -> toy; **4th** -> 10 + 10 = **20$**; 5th -> toy;  |
| 170.00| | **6th** -> 20 + 10 = **30$**; 7th -> toy; **8th** -> 30 + 10 = **40$**; 9th -> toy; **10th** -> 40 + 10 = **50$**.|
| 6| | **Lily saved** -> 10 + 20 + 30 + 40 + 50 = **150$**. She sold **5 toys 6$ each** = **30$**. Her brother took **5 times per 1$ = 5$**.|
| | | **Left money** -> 150 + 30 – 5 = **175$** 175 >= 170**(laundry&#39;s price) **she bought it and are left** 175-170 = **5$**|

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 21 | No! 997.98 | **Lily saved 550$**.  **573 < 1570.98 - Lily had failed to buy a washing machine.**|
| 1570.98| | Her brother took **10 years 1$ each year** = **10$**.|
| 3| | **She sold 11** toys **3$ each** = **33$**.  **Left money** 550 + 33 – 10 = **573$**|
| | | **She needs** 1570.98–573 = **997.98$ more**|

9. \* Histogram

There are given **n integers in the range [1 ... 1000]**. Some percentage of them **p1** are under 200, another percent **p2** are from 200 to 399, another percentage **p3** are from 400 to 599, another percentage **p4** are from 600 to 799 and the other percent **p5** are 800 and more. Write a program that calculates and prints the percentages **p1, p2, p3, p4 and p5.**

**Example** : we have n = **20** numbers: 53, 7, 56, 180, 450, 920, 12, 7, 150, 250, 680, 2, 600, 200, 800, 799, 199, 46, 128, 65. We get the following distribution and visualization:

| **Range** | **Numbers in range** | **Count of numbers** | **Percentage** |
| --- | --- | --- | --- |
| < 200 | 53, 7, 56, 180, 12, 7, 150, 2, 199, 46, 128, 65 | 12 | p1 = 12.0 / 20 \* 100= **60.00%** |
| 200 … 399 | 250, 200 | 2 | p2 = 2.0 / 20 \* 100= **10.00%** |
| 400 … 599 | 450 | 1 | p3 = 1.0 / 20 \* 100= **5.00%** |
| 600 … 799 | 680, 600, 799 | 3 | p4 = 3.0 / 20 \* 100= **15.00%** |
| ≥ 800 | 920, 800 | 2 | p5 = 2.0 / 20 \* 100= **10.00%** |

### **Input**

The **first** line of the input stands **the integer n (1 ≤ n ≤ 1000) - count of numbers**. The **next n** lines contain in an **integer in the range [1 ... 1000]** - the numbers to be **calculated** on the **histogram**

### **Output**

Print on the console the histogram - **5 rows**, each of which contains a **number** between 0% and 100%, **formatted to the second decimal format**, e.g. 25.00%, 66.67%, 57.14%

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   
| --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| **3** | 66.67% || **4** | 75.00% || **7** | 14.29% | 
| 1| 0.00%| | 53| 0.00%| | 800| 28.57%|
| 2| 0.00%| | 7| 0.00%| | 801| 14.29%|
| 999| 0.00%| | 56| 0.00%| | 250| 14.29%|
| | 33.33%| | 999| 25.00%| | 199| 28.57%|
| | | | | | | 399| |
| | | | | | | 599| |
| | | | | | | 799| |


| **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| **9** | 33.33% || **14** | 57.14% |
| 367| 33.33%| | 53| 14.29%|
| 99| 11.11%| | 7| 7.14%|
| 200| 11.11%| | 56| 14.29%|
| 799| 11.11%| | 180| 7.14%|
| 999| | | 450| |
| 333| | | 920| |
| 555| | | 12| |
| 111| | | 7| |
| 9| | | 150| |
| | | | 250| |
| | | | 680| |
| | | | 2| |
| | | | 600| |
| | | | 200| |