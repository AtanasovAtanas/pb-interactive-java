# Exercise: Conditional Statements

1. Even or Odd

Write a program that reads an **integer** from the console and print if it is **even** or **odd**.

### **Example**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | even | | 3 | odd | | 25 | odd | | 1024 | even |

2. 3 Equal Numbers

Read **3** numbers from the console and print if they are **equal** (**yes/no**).

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | yes | | 5 | yes | | 1 | no | | 11 | no | | 13 | no |
| 1 | | | 5 | | | 2 | | | 8 | | | 14 | |
| 1 | | | 5 | | | 3 | | | 5 | | | 99 | |

**\*Hint**: Make a search for boolean operator **"&&"**

3. Area of Figures

Write a program in which the user enters type and dimensions of a geometric figure and calculates its area. Figures are four types: **square, rectangle, circle and triangle**. On the first line of the input you will receive the type of the figure. If it&#39;s **square**, on the next line you will be given a **number** representing **length** of his size. If the type is **rectangle**, on the next **two** lines you have to read its **dimensions**. If it&#39;s **circle** - on the next line you will receive a single number - the **radius**. If the figure is **triangle**, on the next **two** lines you will be given the **length** of its size and the **height** to it. The result should **be formatted to the third decimal point**.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| square | 25.000 | | rectangle | 17.500 | | circle | 113.097 | | triangle | 45.000 |
| 5 | | | 7 | | | 6 | | | 4.5 | |
| | | | 2.5 | | | | | | 20 | |

4. Time + 15 Minutes

Write a program that reads from the console an **hour** and **minutes** from 24-hour day, and calculates what will be the time **after 15 minutes**. Print the result in the following format: **hours:minutes**. The hours will always be between 0 and 23, and the minutes will always be between 0 and 59. The hours are written with one or two digits, the minutes - always with two digits with **leading zero**, if it&#39;s necessary.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1| 2:01 | | 0 | 0:16 | | 23 | 0:14 | | 11 | 11:23 | | 12 | 13:04 |
| 46 | | | 01 | | | 59 | | | 08 | | | 49 | |

5. Day of Week

Write a program that reads an integer from the console and prints **day of the week** (in English) in range **[1… 7]** and **&quot;Error&quot;** if the number is **invalid**.

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 1 | Monday |
| 2 | Tuesday |
| 3 | Wednesday |
| 4 | Thursday |
| 5 | Friday |
| 6 | Saturday |
| 7 | Sunday |
| -1 | Error |

6. Animal Type

Write a program that prints the **type** of an animal according to its **name**.

- **dog -> mammal**
- **crocodile, tortoise, snake -> reptile**
- **others -> unknown**

### **Examples**

| **Input** | **Output** |
| --- | --- |
| dog | mammal |
| snake | reptile |
| cat | unknown |

7. Pets

Martina loves to travel. She has **3 pets** (a dog, a cat and a turtle). When she goes to an adventure, she has to comply with **how much food to leave** them not to stay hungry. Write a **program** calculating the **amount of kilograms** the pets will eat for the time Martina is **on adventure** and **checks if the food is enough**. Each animal eats certain amount food per day.

### **Input**

Read **five** lines from the console:

- First line- **number of days - an integer in range [1…5000]**
- Second line- **left food in kilograms - an integer in range [0…100000]**
- Third line - **food for the dog per day in kilograms - double in range [0.00…100.00]**
- Fourth line - **food for the cat per day in - double in range [0.00…100.00]**
- Fifth line- **food for the turtle per day in grams - double in range [0.00…10000.00]**

### **Output**

Print on the console a **single** line:

- If the left food **IS enough**:
  - **&quot;{kilograms remain} kilos of food left.&quot;**
    - **The result should be rounded to the nearest lower integer**
- If the left food **IS NOT enough**:
  - **&quot;{kilograms needed} more kilos of food are needed.&quot;**
    - **The result should be rounded to the nearest higher integer**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2 | 3 kilos of food left. | **Food needed for:**|
| 10| | **dog** = 2 days \* 1 kg = **2** kg;|
| 1| | **cat** = 2 days \* 1 kg = **2** kg;|
| 1| | **turtle** = 2 days \* 1200 g = **2.4** kg;|
| 1200| | **Total amount of food** = 2 + 2 + 2.4 = **6.4** kg;|
| | | **6.4 < 10** =\&gt; 10 - 6.4 = **3.6** -\&gt; **3 kg food remain**|



| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 5 | 7 more kilos of food are needed. | **Needed food for:** | 
| 10| | **dog** = **10.5** kg;|
| 2.1| | **cat** = 5 days \* 0.8 kg = **4** kg;|
| 0.8| | **turtle** = 5 days \* 321 g = **1.605** kg;|
| 321| | **Total amount of food** = 10.5 + 4 + 1.605 = **16.105** ;|
| | | 16.105 – 10 = 6.105 -> 7 kgof food are needed|

8. Pipes In Pool

A pool with **volume V** has **two pipes** that fill it. **Every pipe has certain flow** (liters water that going through a single pipe per hour). The worker turns on the pipes **at the same time** and goes out for **N hours**. Write a program that shows the condition of the pool **at the moment the worker comes back**.

### **Input**

**Four** lines of input:

- First line - **V** - **The volume of the pool in liters** - integer in range[1…10000].
- Second line - **P1** - **flow of the first pipe per hour** - integer in range[1…5000].
- Third line - **P2** - **flow of the second pipe per hour** - integer in range[1…5000].
- Fourth line - **H** - **hours the worker is missing** - float-pointing number in range [1.0…24.00]

### **Output**

Print on the console **one of both possibilities**:

- How far the pool has been filledand which pipe how much contributed in percentage
  - **&quot;The pool is {occupancy of the pool in percent}% full. Pipe 1: {percent water from the first pipe}%. Pipe 2: {percent water from the second pipe}%.&quot;**
- If the pool is overflowing – how many liters are overflowed for the given time
  - **&quot;For {hours pipes are filling the pool} hours the pool overflows with {liters water overflow} liters.&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 1000| The pool is 66.00% full. Pipe 1: 45.45%. Pipe 2: 54.55%. | For 3 hours: The first pipe fills up 300 liters|
| 100| | The second pipe fills up 360 liters|
| 120| | In total – 660 l < 1000 l => 66% are filled up|
| 3| | The first pipe is contributed with 45% (300 of 660 liters).|
| | | The second pipe is contributed with 54% (360 of 660 liters).|


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 100 | For 2.50 hours the pool overflows with 400.00 liters. | For 2.5 hours: The first pipe fills up 250 l |
| 100| | The second pipe fills up 250 l|
| 100| | In total – 500 l > 100 l => 400 l are overflowed.|
| 2.5| | |

# Examples for Exam Problems

9. \* Toy Shop

Monica has a toy shop. She receives a big order and she has to perform it. With the money she win, Monica wants to go on a vacation. Write a program that calculates the profit from the order.

**Prices of the toys**:

- **Puzzle - 2.60 $**
- **Talking doll - 3 $**
- **Teddy Bear - 4.10 $**
- **Minion - 8.20 $**
- **Truck - 2 $**

If the ordered toys are **50 or more**, the shop applies **25% discount from the total price**. **10%** of the raised money Monica has to give for shop&#39;s **rent**. Calculates if the money will be enough for Monica to go on a vacation.

### **Input**

Read **6** lines of input from the console:

1. **Price of the vacation - double number in range [1.00…10000.00]**
2. **Count of puzzles - integer in range [0…1000]**
3. **Count of talking dolls - integer in range [0…1000]**
4. **Count of Teddy Bears - integer in range [0…1000]**
5. **Count of minions - integer in range [0…1000]**
6. **Count of trucks - integer in range [0…1000]**

### **Output**

Print on the console:

- If the money **are** enough, print the following message:
  - **&quot;Yes! {money left} dollars left.&quot;**
- If the money are **NOT** enough:
  - **&quot;Not enough money! {money needed} dollars needed.&quot;**

**The result should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | **Comment** |
| --- | --- | --- |
| 40.8| Yes! 418.20 dollars left. | **Total sum**: 20 \* 2.60 + 25 \* 3 + 30 \* 4.10 + 50 \* 8.20 + 10 \* 2 = **680** $     |
| 20| | **Count of the toys** : 20 + 25 + 30 + 50 + 10 = **135**|
| 25| | **135 > 50 => 25%** discount;|
| 30| | 25% of 680$ = **170 $ discount** |
| 50| | **End price**: 680 – 170 = **510 $**|
| 10| | **Rent**: 10% of 510$ = **51 $**|
| | | **Profit** : 510 – 51 = **459 $**|
| | | **459 > 40.8** => 459 – 40.8= **418.20 $ left**|




| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 320 | Not enough money! 238.73 dollarsneeded. | **Total sum**: **90.3 $** |
| 8| | **Count of the toys**: 21 |
| 2| | **21 < 50 => there isn&#39;t a discount**|
| 5| | **Rent**: 10% of 90.3 = **9.03 $**|
| 5| | **Profit**: 90.3 – 9.03 = **81.27 $**|
| 1| | **81.27 < 320** => 320 – 81.27= **238.73 $ needed**|