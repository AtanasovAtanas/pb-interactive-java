# Exercise: Conditional Statements Advanced

1. Personal Titles

Write a **console**** program **that reads** age**(floating-point number) and **gender**(&quot;**m **&quot; or &quot;** f**&quot;) and prints **address** among these:

- &quot; **Mr.**&quot;- a man (gender&quot; **m**&quot;) of age 16 or more
- &quot; **Master**&quot;- a boy (gender &quot; **m**&quot;) under 16 years old
- &quot; **Ms.**&quot;- a woman (gender&quot; **f**&quot;) of age 16 or more
- &quot; **Miss**&quot;- a girl (gender&quot; **f**&quot;) under 16 years old

### **Examples**

| **Input** | **Output** |      
| --- | --- |                   
| 12 | Miss |                   
| f | |   

| **Input** | **Output** | 
| --- | --- |
| 17 | Mr. |
| m | |

| **Input** | **Output** | 
| --- | --- |
| 25 | Ms. |
| f | |

| **Input** | **Output** | 
| --- | --- |
| 13.5 | Master |
| m | |

2. Fruit or Vegetable

Your task is to write a program that takes as input from the user **name of a product** and checks if the product is **fruit** or **vegetable**.

- The fruits &quot;**fruit**&quot; are **banana**, **apple**, **kiwi**, **cherry**, **lemon** and **grapes**
- The vegetables &quot;**vegetable**&quot; are **tomato**, **cucumber**, **pepper** and **carrot**
- Everything else is &quot;**unknown**&quot;

Print on the console &quot;**fruit**&quot;, &quot;**vegetable**&quot; or&quot;**unknown**&quot; according to the product name.

### **Examples**

| **Input** | **Output** |      
| --- | --- |                   
| banana | fruit |                   

| **Input** | **Output** |      
| --- | --- |                   
| tomato | vegetable | 

| **Input** | **Output** |      
| --- | --- |                   
| water | unknown | 

\* **Hint** : use conditional **if** statement with logical &quot;**or**&quot; - operator **||**.

3. Trade Commissions

A company gives the following **commissions** to its businessmen according to the **city** they work in and the **amount** of **sales** **s**:

| **City** | 0 ≤ s ≤ 500 | 500 < s ≤ 1000 | 1000 < s ≤ 10000 | s > 10000 |
| --- | --- | --- | --- | --- |
| London | 5% | 7% | 8% | 12% |
| New York | 4.5% | 7.5% | 10% | 13% |
| Sydney | 5.5% | 8% | 12% | 14.5% |

Write a **console** program **that reads as input the** name of a **city** (String) and the **amount of sales** (floating-point number) and calculates and prints the value of the **trade commission**. You can help yourself using the table above. The result should be **formatted to the second decimal point**. If you receive **invalid** name of city or amount of sales (negative number), print **&quot;error&quot;**.

### **Examples**

| **Input** | **Output** | **Input** | **Output** | **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| London | 120.00 | Sydney | 27.50 | New York | 387.45 | Moscow | error |
| 1500 | | 499.99 | | 3874.50 | | -50 | |

4. Point on Rectangle Border

Write a program to check is a **point {x, y}** is **on** some of the sides of a rectangle **{x1, y1} – {x2, y2}**. The input comes from the console and it consists of **6 rows, introduced from the user: real numbers x1, y1, x2, y2, x and y** (it will be always true that **x1 < x2** and **y1 < y2**). Print **&quot;Border&quot;** (the point lies on one of the sides) or **&quot;Inside / Outside&quot;** (otherwise).

### **Examples**

| **Input** | **Output** | **Input** | **Output** | 
| --- | --- | --- | --- | --- | 
| 2 | Inside / Outside | 2 | Border |
| -3 | | -3 | |
| 12 | | 12 | |
| 3 | | 3 | |
| 8 | | 12 | |
| -1 | | -1 | | 

\* **Hint** : use one or more conditional **if** statements with logical operations. A point **{x, y}** lies on aside of a rectangle **{x1, y1} – {x2, y2}**, if it's fulfilled one of the specified conditions:

- **x** equals **x1** or **x2** and at the same time **y** is between **y1** and **y2**
- **y** equals **y1** or **y2** and at the same time **x** is between **x1** and **x2**

You can check the conditions above using one more complicated **if**-**else** construction or using few more simple conditional statements or **nested if**-**else statements.**

5. Summer Outfit

It's summer with changeable weather and Victor need your help. Write a program that recommends Victor which clothes to choose **according to the part of day and degrees (Celsius)**. Your friend has different plans for every part of the day with different outfits – check the **table** below.

### **Input**

**Read two lines of input:**

- **Degrees - an integer in range [10…42]**
- **Text - part of day - possibilities: &quot;Morning&quot;, &quot;Afternoon&quot;, &quot;Evening&quot;**

| **Part of day**  **/**  **Degrees** |  Morning |  Afternoon |  Evening |
| --- | --- | --- | --- |
| 10 <= degrees <= 18 | Outfit = Sweatshirt | Outfit = Shirt | Outfit = Shirt |
| | Shoes = Sneakers | Shoes = Moccasins | Shoes = Moccasins |
| 18 <  degrees <= 24 | Outfit = Shirt | Outfit = T-Shirt | Outfit = Shirt |
| | Shoes = Moccasins | Shoes = Sandals | Shoes = Moccasins |
| degrees >= 25 | Outfit = T-Shirt | Outfit = Swim Suit | Outfit = Shirt |
| | Shoes = Sandals | Shoes = Barefoot | Shoes = Moccasins |

### **Output**

- Print on the console a **single** line: **&quot;It's {degrees} degrees, get your {outfit} and {shoes}.&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 16 | It&#39;s 16 degrees, get your Sweatshirt and Sneakers. | In the morning when the degrees are 16, |
| Morning | | Victor takes a sweatshirt and sneakers.|
| **Input** | **Output** | |
| 22 | It&#39;s 22 degrees, get your T-Shirt and Sandals. |  |
| Afternoon | | |
| **Input** | **Output** | |
| 28 | It&#39;s 28 degrees, get your Shirt and Moccasins. ||
| Evening | | |

6. Fishing Boat

Tony and his friends loves to go fishing and because of that they&#39;ve decided to go fishing with boat. The rent of the boat depends on the **season** and the **number** of fishermen.

**The price** on the basis of **season**:

- **Spring - 3000 $**
- **Summer and autumn - 4200 $**
- **Winter - 2600 $**

**The price** on the basis of **number** of fishermen uses **discount:**

- If the group is **up to 6 people (inclusive) -  10% discount**
- If the group members are in range **[7…11] -  15% discount**
- If the group is **12 or more people - 25% discount**

The fishermen use another **5 % discount if they are even number** except when it is **NOT** autumn – then they do **NOT** have additional discount.

Write a **program** to **calculate** whether the fishermen will gather **enough** money.

### **Input**

The input is consists of exactly **3 lines**:

- The **budget** of the group - **real number in range [1…8000]**
- **Season**  - String : **&quot;Spring&quot;**, **&quot;Summer&quot;**, **&quot;Autumn&quot;**, **&quot;Winter&quot;**
- **Number** of fishermen - **integer in range [4…18]**

### **Output**

Print on the console a **single** line:

- If the budget **IS** enough:

**&quot;Yes! You have {money left} dollars left.&quot;**

- If the budget **IS NOT** enough:

**&quot;Not enough money! You need {money needed} dollars.&quot;**

**The prices should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 3000 | Not enough money! | In the summer fishing costs 4200$, |
| Summer | You need 570.00 dollars. | **11 fishermen take 15% discount** -> **4200 - 15% = 3570** $, |
| 11 | | their number is **odd** so they do **not** use **additional** discount. |
| | | 3000 <= 3570, hence they need 570.00 $ more |


| **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- |
| 3600 | Not enough money! | 2000 | Yes! You have 50.00 dollars left. |
| Autumn | You need 180.00 dollars. | Winter | |
| 6  | | 13 |

7. Flowers

A flower market offers **3 types of flowers: chrysanthemum** , **roses** and **tulips**. The prices depends on the season.

| **Season** | **Chrysanthemum** | **Rose** | **Tulip** |
| --- | --- | --- | --- |
| **Spring**  **/**  **Summer** | **2.00 $** | **4.10 $** | **2.50 $** |
| **Autumn**  **/**  **Winter** | **3.75 $** | **4.50 $** | **4.15 $** |

In the holidays the prices of all flowers **increase by 15%**. The market offers the following **discounts** :

- If you buy **7 or more tulips during the spring** - **5% of the price of the whole bouquet**
- If you buy **10 or more roses during the winter** - **10% of the price of the whole bouquet**
- If you buy **more than 20 flowers in total during ALВ seasons - 20% of the price of the whole bouquet**

**The discounts are applied in the specified order above and can be superimposed! All of the discounts should be applied after the increasing of the prices in holidays!**

The price of the bouquet arrangement is **always** 2 dollars. Write a program to **calculate** the price of a bouquet.

### **Input**

The input is read from the **console** and is exactly **5 lines** :

- First line - count of the bought **chrysanthemum** - **integer in range [0 ... 200]**
- Second line - count of the bought **roses** - **integer in range [0 ... 200]**
- Third line - count of the bought **tulips** - **integer in range [0 ... 200]**
- Fourth line - **season** - **[Spring, Summer, Аutumn, Winter]**
- Fifth line - if the day is **holiday** - **[Y - yes / N - no]**

### **Output**

Print on the console a **single number** - **the**** price of the flowers, formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2 | 46.14 | **Price: 2\*2.00 + 4\*4.10 + 8\*2.50 = 40.40 $** |
| 4 | | **Holiday**  40.40 + **15%** =46.46 $|
| 8 | | **5% discount for more than 7 tulips during the spring** - 44.14|
| Spring | | In total the flowers are 20 or less - there **isn't a discount**|
| Y | | **44.14 + 2 for arrangement = 46.14 $** |


| **Input** | **Output** | **Comment** | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 3 | 69.39 | **Price**: 3\*3.75 + 10\*4.50 + 9\*4.15 = **93.60 $** | 10 | 101.20 |
| 10 | | **It is NOT a holiday - there is not increment** | 10 | |
| 9 | | **10 % discount for 10 or more roses during the winter - 84.24** | 10 | |
| Winter | | In total the flowers are more than 20 - 20% discount = **67.392**| Autumn | |
| N | | **67.392 + 2 for arrangement = 69.392 $** | N | |

# 2. Examples for Exam Problems

8. Journey

It's strange, but most of the people plan their vacation early. A young programmer has **concrete budget** and **free time** in a certain **season**. Write a program that receives as an **input** the **budget** and the season, and as **output** prints **where** will be the programmer's **vacation** and **how much he will** spend.

**The budget determines the destination, the season - how much from the budget will be spend**. If it is **summer**, the programmer will rest at **camping** , if it's **winter** - in a **hotel**. If he is in **Europe** independent **of the season**, he will stay in a **hotel**. Every **camping** or **hotel**, according to the **destination**, has its **own price** that corresponds to a **percentage of the budget**:

- Budget **100 $ or less** - somewhere in **France**
  - **Summer** - **30%** of the budget
  - **Winter** - **70%** of the budget
- Budget **1000 $ or less**  - somewhere in **USA**
  - **Summer** - **40%** of the budget
  - **Winter** - **80%** of the budget
- Budget **more than 1000 $** - somewhere in Europe
  - If he travels in Europe, **independent** of the season, he will spend **90% of the budget**

### **Input**

The input comes from the console as **two lines**:

- First line - **budget - real number in range [10.00...5000.00]**
- Second line - one of two possible seasons: **&quot;summer&quot;** or **&quot;winter&quot;**

### **Output**

You have to print **two lines**:

- First line - **&quot;Somewhere in [destination]&quot;** among **&quot;France&quot;**, **&quot;USA&quot;** and **&quot;Europe&quot;**
- Second line - **&quot;{type of place to stay} – {spend money}&quot;**
  - **Type of place to stay** will be **&quot;Camp&quot;** or **&quot;Hotel&quot;**
  - **The amount of spend money** should be **formatted to the second decimal point**

### **Examples**

| **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- |
| 50 | Somewhere in France | 75 | Somewhere in France |
| summer | Camp - 15.00 | winter | Hotel - 52.50 |

| **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- |
| 312 | Somewhere in USA | 678.53 | Somewhere in USA |
| summer | Camp - 124.80 | winter | Hotel - 542.82 |

| **Input** | **Output** |
| --- | --- |
| 1500 | Somewhere in Europe |
| summer | Hotel - 1350.00 |

9. Operations Between Numbers

Write a program that reads **two integers (N1 and N2)** and an **operator** that defines the **mathematical operation** you have to make with the given numbers. The possible operations are: **addition (+)**, **subtraction (-)**, **multiplication (\*)**, **division (/)** and **modulus division (%)**. In case of addition, subtraction and multiplication you have to print the **result** and whether it's **even** or **odd**. In case of simple **division** - print only the **result**. In case of **modulus division**- print the **remainder**.You should keep in mind that the **divisor could be 0 (zero)**, and as you know - you **cannot divide by 0**. In that case you have to print a **special message**.

### **Input**

The input is consists of the following **3 lines**:

- **N1 - integer in range [0...40000]**
- **N2 - integer in range [0...40000]**
- **Operator - one of the symbols: '+', '-', '\*', '/', '%'**

### **Output**

Print on the console a **single** line:

- If the operation is **addition, subtraction or multiplication**:
  - **&quot;{N1} {operator} {N2} = {result} – {even/odd}&quot;**
- If the operation is **division**:
  - **&quot;{N1} / {N2} = {result}&quot;** - where the result is formatted to the **second decimal point**
- If the operation is **modulus division**:
  - **&quot;{N1} % {N2} = {remainder}&quot;**
- In case of **division by 0 (zero)**:
  - **&quot;Cannot divide {N1} by zero&quot;**

### **Examples**

| **Input** | **Output** | **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- |
| 10 | 10 + 12 = 22 - even | 123 | 123 / 12 = 10.25 | 112 | Cannot divide 112 by zero |
| 12 | | 12 | | 0| |
| + | | / | | / | |

| **Input** | **Output** | **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- |
| 10 | 10 – 1 = 9 - odd | 10 | 10 % 3 = 1 | 10 | Cannot divide 10 by zero |
| 1 | | 3 | | 0 |
| - | | % | | % | 