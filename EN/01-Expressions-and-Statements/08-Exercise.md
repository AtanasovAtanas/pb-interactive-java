## Exercise: Expressions and Statements

1. Square Area

Write a console program that reads an **integer** &#39;a&#39; and calculates the **area** of a square with size &#39;a&#39;.

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 5 | 25 |

2. Projects Creation

Write a program that calculates how many hours will be necessary to an architect to create projects of someconstruction objects. Creating one project takes approximately 3 hours.

### **Input**

Read **two** lines from the console:

1. **Name of the architect - String**
2. **Number of projects - integer in range [0… 100]**

### **Output**

Print on the console:

- **&quot;The architect {name of the architect} will need {necessary hours} hours to complete {number of projects} project.&quot;**

### **Examples**

| **Input** | **Output** |  
| --- | --- |
| George | The architect George will need 12 hours to complete 4 project/s. |
| 4 | |

| **Input** | **Output** |  
| --- | --- |
| Sanya | The architect Sanya will need 27 hours to complete 9 project/s. |
| 9 | |

3. Trapezoid Area

Write a program that reads **three** numbers **b1** , **b2** and **h** and calculates the **area** of trapezoid with **bases b1 and b2** and **height h**. 

The formula for calculating **area** of a trapezoid is **((b1 + b2) / 2) * h**.

For example if we have a trapezoid with bases 8 and 13 and height 7, it will have area (8 + 13) \* 7 / 2 = 73.5.

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 8 | 73.50 |
| 13 | |
| 7 | |

4. Vegetable Market

Gardener is selling his harvest at the vegetable market. He sells **vegetables for N dollars per kilogram** and **fruits for M dollars per kilogram**. Write a program that **calculates the income** from the harvest in **euros** (**1 USD = 0.89 EUR**).

### **Input**

The input will be **4 numbers**, each on a single line:

- First line - **The price of kilogram vegetables** - **floating-point number [0.00… 1000.00]**
- Second line - **The price of kilogram fruits** - **floating-point number [0.00… 1000.00]**
- Third line - **The total kilograms of vegetables** - **integer [0… 1000]**
- Fourth line - **The total kilograms of fruits** - **integer [0… 1000]**

### **Output**

Print on the console **a single number**: the income from **all** of the fruits and vegetables in **euro**.

**The result should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 0.194 | 174.39 | The vegetables cost - 0.194$ \* 10kg = 1.94$ |
| 19.4 | | The fruits cost - 19.4$ \* 10kg  = 194$ |
| 10 | | Total - 195.94$ = 174.39€ |
| 10 | | |

| **Input** | **Output** |
| --- | --- |
| 1.5 | 35.60 |
| 2.5 | |
| 10 | |
| 10 | |

5. Fishland

George will have guests this evening and decides to feed them with **tuna, scads** and **mussels**. That&#39;s why he goes to the Fishland to buy some kilograms **fish**. From the console are read the prices **of mackerel and sprats**.  Also you will be given the **quantity of tuna**, **scads and mussels** in **kilograms**. **How much money** will he need to pay his bill, if the **prices** at the Fishland are:

- Tuna - **60% more expensive than the mackerel**
- Scads - **80% more expensive than the sprats**
- Mussels - **7.50 dollars per kilogram**

### **Input**

You have to read **5** numbers from the console:

- First line - **the price of the mackerel per kilogram - floating-point number in range [0.00…40.00]**
- Second line - **the price of the sprats per kilogram - floating-point number in range [0.00…30.00]**
- Third line - **kilograms of tuna - floating-point number in range [0.00…50.00]**
- Fourth line - **kilograms of scads - floating-point number in range [0.00…70.00]**
- Fifth line - **kilograms of mussels - integer number in range [0...100]**

### **Output**

Print on the console a **single** number with floating point: **the money** George will need to pay the bill, **formatted to the second decimal point** (1.2457 -> 1.25).

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 6.90 | 42.96 | The price of the tuna = 6.90 + 6.90 \* 0.60 = 11.04 $/kg |
| 4.20 | | Total sum of tuna = 1.5 \* 11.04 = 16.56 |
| 1.5 | | The price of the scads = 4.20 + 4.20 \* 0.80 =  7.56$/kg |
| 2.5 | | Total sum of scads = 2.5 \* 7.56 = 18.90 |
| 1 | | The total sum of mussels = 1 \* 7.50 = 7.50 |
| | | Bill = 16.56 + 18.90 + 7.50 = 42.96 |


| **Input** | **Output** |
| --- | --- |
| 5.55 | 113.82 |
| 3.57 | |
| 4.3 | |
| 3.6 | |
| 7 | |

| **Input** | **Output** |
| --- | --- |
| 7.79 | 115.92 |
| 5.35 | |
| 9.3| |
| 0 | |
| 0 | |

6. Pet Shop

Write a program that **calculates the expenses** for buying food for dogs. The food is bought **mainly for dogs** from the pet shop, but sometimes the dogs&#39; owner buys food and for **his neighbor&#39;s animals**. Each package of **food for dogs costs 2.5 dollars**, and every **other that&#39;s NOT for them - 4 dollars**.

### **Input**

The input will be **two** lines from the console:

1. Number of dogs - **integer in range [0… 100]**
2. Number of the others animals - **integer in range [0… 100]**

### **Output**

Print on the console:

**&quot;{total sum} dollars&quot;**

**The result should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 5 | 28.50 dollars |
| 4 | |


| **Input** | **Output** |
| --- | --- |
| 13 | 68.50 dollars |
| 9 | |

7. Yard Greening

Katrine has a **few** houses on the East Coast and she wants to landscape the yards of some of them. For that reason she rents a company.

Write a program that **calculates the expenses** Katrine has to pay to the company. The price **for one square meter is 7.61 dollars with VAT**. The company offers **18% discount from the total price** , because Katrine&#39;s yard is big.

### **Input**

Single line from the console:

- **Square meters** which will be greening - **float-pointing number in range [0.00… 10000.00]**

### **Output**

Print on the console **two lines** :

- **&quot;The final price is: {total price} dollars&quot;**
- **&quot;The discount is: {discount} dollars&quot;**

**Both** prices should be formatted to the **second decimal point**.

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 540  | The final price is: 3369.71 dollars | Calculate the price for greening the whole yard: |
| | The discount is: 739.69 dollars | 540 \* 7.61 = 4109.40$|
| | | Calculate the discount: |
| | | 0.18 \* 4109.40 = 739.69$ |
| | | Calculate the final price: |
| | | 4109.40 – 739.69 = 3369.71$|


| **Input** | **Output** |
| --- | --- |
| 135  | The final price is: 842.43 dollars |
| | The discount is: 184.92 dollars |

## 2. Examples of Exam Problems

8. \* Fish Tank

For his birthday Tom receives a fish tank in form of parallelepiped. **First** , read from the console its **dimensions** , **each on a separate line - length, width, height in cm**. You have to calculate how many liters water the tank will hold, if you know that certain percent of its volume it&#39;s taken with sand, plants, heater and a pomp.

One liter water equals one cubic decimeter ( **1l = 1 dm<sup>3</sup>**).

**Write a program that calculates water liters necessary to full the fish tank.**

### **Input**

**Four** lines from the console:

1. **Length** in cm - **integer in range [10…500]**
2. **Width** in cm - **integer in range [10…300]**
3. **Height** in cm - **integer in range [10…200]**
4. **Percent** - **floating-point number in range [0.000…100.000]**

### **Output**

Print on the console a **single** number:

- **Liters of water the tank will holds, formatted to the third decimal point.**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 85 | 248.689 | Calculate the **volume** of the **tank**:  |
| 75 | | **volume** = 85\*75\*47= **299625** cm<sup>3</sup> |
| 47 | | **Total liters to hold:** 299625 \* 0.001= **299.625** liters |
| 17 | | **Percent** : **17**\*0.01= 0.17 |
| | | **Liters you&#39;ll need in fact:** 299.625\*(1-0.17) = **248.68875 liters** |



| **Input** | **Output** |
| --- | --- |
| 105 | 586.445 |
| 77 | |
| 89 | |
| 18.5 | |


9. \* Charity Campaign

There is a charity campaign in the bakery in which bakers from all the country can take part. First we read the **number of days** of the campaign and the **number of bakers** who will take part. After that **on separate lines** we receive the **amount of the cakes, waffles and pancakes that will be prepared by one baker for one day**. You should have in mind the following prices:

- **Cake - 45$**
- **Waffle - 5.80$**
- **Pancake - 3.20$**

**1/8 from the total price will be for expenses for products, used in the campaign.**

Write a program to calculate the **total sum** at the end of the charity campaign.

### **Input**

Read **5** lines from the console:

1. Number of **days** of campaign - **integer in range [0…365]**
2. Number of **bakers - integer in range [0…1000]**
3. Number of **cakes - integer in range [0…2000]**
4. Number of **waffles - integer in range [0…2000]**
5. Number of **pancakes  - integer in range [0…2000]**

### **Output**

Print on the console a **single** number:

- **The money, raised from the charity campaign, formatted to the second decimal point**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 20 | 119728.00 | Calculate the **amount of money** earn **per day** for **each of the products**, made by **one baker**: |
| 8 | | **Cakes** : 14 \* 45 = **630 $**|
| 14 | | **Waffles** : 30 \* 5.80 = **174 $**|
| 30 | | **Pancakes**: 16 \* 3.20 = **51.20 $**|
| 16 | | **Total sum per day**: (630 + 174 + 51.20) \* 8 = **6841.60 $**|
| | | **The sum raised from the campaign**: 6841.60 \* 20 = **136832 $**|
| | | **The sum after covering the expenses**: 136832 - 1/8 от 136832 = **119728 $**|

| **Input** | **Output** |
| --- | --- |
| 131 | 426175.75 |
| 5 | |
| 9 | |
| 33 | |
| 46 | |