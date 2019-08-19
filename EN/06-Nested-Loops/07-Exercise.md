# Exercise: Nested Loops

1. Numbers 1...N with Step 3

Write a program that reads a **number n**, introduced by the user, and prints **the numbers from 1 to n in 3 (step 3)**.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 10 | 1 | | 7 | 1 | | 15 | 1 |
| | 4 | | | 4 | | | 4 |
| | 7 | | | 7 | | | 7 |
| | 10 | | | | | | 10 |
| | | | | | | | 13 |

2. Combinations

Write a program that calculates **how many solutions in natural numbers (including zero)** has the equation:

**x1 + x2 + x3 + x4 + x5 = n**

**The number n is an integer and is entered from the console.**

### **Examples**

| **Input** | **Output** | **Comments** | 
| --- | --- | --- |
| 25 | 23751 | Generate all combinations of 5 digits, the first is: |
| | | 0+0+0+0+0=0, but because it is not equal to 25, continuing|
| | | 0+0+0+0+1=1 - again, it&#39;s not 25, etc. |
| | | We come to the first valid combination: |
| | | 0 + 0 + 0 + 0 + 25 = 25, expanding the number of valid combinations of 1,|
| | | the second valid combination is:| 
| | | 0 + 0 + 0 + 1 + 24 = 25|
| | | The third:0 + 0 + 0 + 2 + 23 = 25  etc.|
| | | After generating all possible combinations,|
| | | the number of valid is 23751.|

| **Input** | **Output** | | **Input** | **Output** | 
| --- | --- | --- | --- | --- |
20 | 10626 | | 5  | 126 |


3. Travelling

Annie likes to travel and she wants this year to visit **several** different destinations. When she choose a destination, she will decide how **much money she&#39;ll need** to go there and she will **start saving money**. When she saved **enough**, she will be able to travel.

### **Input/Output**

- From the **console** every time will be **read first destination and the minimum budget** which will be needed for the trip.
- It will then be read a **few sums** that Annie saves while working and **when she succeed in saving enough** for the trip, **she will go**, **as you should print on the console the following message**:

**&quot;Going to {destination}!&quot;**

- When Annie visit all the destinations she wants, **instead of destination she will enter &quot;End&quot;** and the program will end.

### **Examples**

| **Input** | **Output** | **Input** | **Output** |
| --- | --- | --- | --- |
| Greece | Going to Greece! | France | Going to France! |
| 1000 | Going to Spain! | 2000 | Going to Portugal! |
| 200 | | 300 | Going to Egypt! |
| 200 | | 300 | |
| 300 | | 200 | |
| 100 | | 400 | |
| 150 | | 190 | |
| 240 | | 258 | |
| Spain | | 360 | |
| 1200 | | Portugal | |
| 300 | | 1450 | |
| 500 | | 400 | |
| 193 | | 400 | |
| 423 | | 200 | |
| End | | 300 | |
| | | 300 | |
| | | Egypt | |
| | | 1900 | |
| | | 1000 | |
| | | 280 | |
| | | 300 | |
| | | 500 | |
| | | End | |


4. Word Wars

Write a program that **calculates the ASCII value of a few words**, as the word with the **highest value** is the winner. The value of a word is calculated when you sum the **ASCII values of all the letters of which it consists of**. From the console read words until the command **quot;STOP&quot;**, then print:

**&quot;Winner is {winner word} – {value of the word}!&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| House| Winner is Destination - 1154! | The first letter is H and it&#39;s ASCII value is 72, |
| Dog | | o has value 111, |
| Destination | | u has value 117,|
| STOP | | s has value 115, |
| | | e has value 101.|
| | | Their sum is 516.|
| | | Keep doing the same calculations for the other words|
| | | and get that Destination has the highest value - 1154.|

| **Input** | **Output** |
| --- | --- |
| Cat | Winner is Information - 1158! | 
| Doll | | 
|Information | | 
| Winner | | 
| STOP | |


5. Coding

Write a program that reads **an integer** from the console. The console should print **as many lines as digit is number**. As the **first line** of the corresponding **units**, of the second - **tens**, third order - **hundreds** of number, etc., as there are **no more digits** of the number. Each line you must print **symbol**, which satisfies the following conditions:

- The symbol, which must be printed on a line, is located on the [ASCII](http://www.asciitable.com/) table. Its **decimal ASCII code** is calculated as adding **33** to the digit of the input number that corresponds to a given row
- The symbol shall be printed **as many times as the digit** corresponding to this line
- If for a given row **matches a digit 0**, on this line is printed &quot;ZERO&quot;once**


### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2049 | \*\*\*\*\*\*\*\*\* | The number 2049 has four digits so we will print four rows. |
| | %%%% | The first line corresponds to the digit 9. We add 33 to 9 and get 42.|
| | ZERO | This is the decimal ASCII code of the symbol it should be print on the first row.|
| | ## | From the ASCII table we find out that of the 42 corresponds symbol '\*'. |
| | | Because the first line corresponds with digit 9 we print 9 times '\*'. |
| | | For the second line the digit is 4. 4+33=37. Using ASCII table we find that |
| | | the symbol to print is '%'. We print 4 times '%'. |
| | | On the third line matches a digit 0. In this case we do **NOT** searching |
| | | anything in ASCII table and on this line we print ZERO once.|
| | | The last digit of the number is 2. 2+33=35. |
| | | From the ASCII table we found the symbol to print - '#' and we print it twice. |


| **Input** | **Output** | | **Input** | **Output** |
| --- | --- | --- | --- | ---  |
| 9347439 | \*\*\*\*\*\*\*\*\* | | 123456789 | \*\*\*\*\*\*\*\*\*&quot; |
| | $$$ | | | )))))))) |
| | %%%% | | | ((((((( |
| | ((((((( | | | ''''''|
| | %%%% | | | &&&&& |
| | $$$ | | | %%%% |
| | \*\*\*\*\*\*\*\*\* | | | $$$|
| | | | | ## |
| | | | | '' |

**Hints** :
- Read the number as a String, save its length in a variable using the **length() method.** Find more **information** about it in Internet
- To take the last digit of the number, divide it modular of 10 (**num % 10**) and save it in a variable. Then **remove the last digit of the number**, dividing it by 10 (**num / 10**) for the next time again to grab the last digit

6. Train the trainers

The course &quot;Train the trainers&quot; is ending and the final evaluation approaches. Your task is to help the jury which will evaluate the presentations, writing a program to calculate the **average score** of **each presentation** by a student, and the **average of all of them**.

### **Input**

- From the console of the first row read the number of people on the jury - **n** - **an integer in the range [1...20]**
- Then on a separate line read the name of the presentation - **String**
- For each presentation of the new line is read **n - the number of ratings - real number in the interval [2.00 ... 6.00]**

### **Output**

- After calculating the **average score** for a particular presentation, print to the console:

   **&quot; {name of the presentation} - {average score}.&quot;**

- After receiving the command **&quot;Finish&quot;** on the console, print 

**&quot;Student&#39;s final assessment is {average presentations of all presentations}.&quot;**
and the program ends.

All scores must be formatted to the **second decimal point**.

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2 | While-Loop - 5.75. | 2 – the number of people on the jury - therefore |
| While-Loop | For-Loop - 5.75. | gain a 2 evaluations of the presentation|
| 6.00 | Student&#39;s final assessment is 5.75.| (6.00 + 5.50) / 2 = 5.75|
| 5.50 | | (5.84 + 5.66) / 2 = 5.75|
| For-Loop | | (6.00 + 5.50 + 5.84 + 5.66) / 4 = 5.75 |
| 5.84 | | |
| 5.66 | | |
| Fisnish | | |

| **Input** | **Output** | | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 3 | Arrays - 4.92. | | 2 | Objects and Classes - 5.00. |
| Arrays| Lists - 5.75.| | Objects and Classes| Dictionaries - 4.82.|
| 4.53| Student's final assessment is 5.34.| | 5.77| RegEx - 3.15.|
| 5.23| | | 4.23| Student's final assessment is 4.32.|
| 5.00| | | Dictionaries| |
| Lists| | | 4.62| |
| 5.83| | | 5.02| |
| 6.00| | | RegEx| |
| 5.42| | | 2.88| |
| Finish| | | 3.42| |
| | | | Finish| |


7. Lucky Numbers

Write a program that reads **an integer N** and generates all the possible **&quot;lucky&quot;** and **various 4-digit numbers** (each digit of the number is in the range **[1...9]**).  The number must comply with the following **conditions**:

Lucky number is a 4-digit number for which **the sum of the first two digits is equal to the sum of the last two**. The number **N** must be divisible by **no residue** from **the sum** of the first two digits of the **&quot;lucky&quot; number.**

### **Input**

The input is read from the console and consists of **an integer in the range [2 .. 10,000]**

### **Output**

Print on the conole **all &quot;happy&quot; and various 4-digit numbers**, separated by a space

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 3 | 1212 1221 2112 2121 | All of the four numbers are &quot;lucky&quot; |
| | | 3 / (1+2) = 1 – residue 0|
| 7 | 1616 1625 1634 1643 1652 1661 2516 2525 2534 2543 2552 2561 3416 3425 3434 3443 3452 3461 4316 4325 4334 4343 4352 4361 5216 5225 5234 5243 5252 5261 6116 6125 6134 6143 6152 6161 | All numbers are &quot;lucky&quot; |
| | | 7 / (1+6) = 1 – residue 0|
| | | 7 / (2+5) = 1 – residue 0|
| | | 7 / (3+4) = 1 – residue 0|
| 24 | 1111 1212 1221 1313 1322 1331 1515 1524 1533 1542 1551 1717 1726 1735 1744 1753 1762 1771 2112 2121 2213 2222 2231 2415 2424 2433 2442 2451 2617 2626 2635 2644 2653 2662 2671 3113 3122 3131 3315 3324 3333 3342 3351 3517 3526 3535 3544 3553 3562 3571 3939 3948 3957 3966 3975 3984 3993 4215 4224 4233 4242 4251 4417 4426 4435 4444 4453 4462 4471 4839 4848 4857 4866 4875 4884 4893 5115 5124 5133 5142 5151 5317 5326 5335 5344 5353 5362 5371 5739 5748 5757 5766 5775 5784 5793 6217 6226 6235 6244 6253 6262 6271 6639 6648 6657 6666 6675 6684 6693 7117 7126 7135 7144 7153 7162 7171 7539 7548 7557 7566 7575 7584 7593 8439 8448 8457 8466 8475 8484 8493 9339 9348 9357 9366 9375 9384 9393 |   |

8. Safe Passwords Generator

Tom is afraid of this to not be hacked some of the profiles on social networks, so he decided to make a generator for passwords to be secure enough. Your task is to help him to write a program that will generate these passwords, separated by **&#39;|&#39;**.

Write a program that generates a series of characters as in the **template**:

ABxyBA

as each generation of new code, the values of the symbols shall be increased by **1**. If you exceed A **55** , returns of 35. If B **has exceeded 96**, comes back on 64.

### **Input**

Read from the console **three** lines:

- The first line **a**  - an integer in the range [1 ... 1000]
- The second line **b** - in the range[1 … 1000]
- The third row **maximum number of generated passwords** - an integer in the range [1 … 1000000]

### **Constraints**:

- A is a **symbol with ASCII value in the range [35… 55]**
- B is a **symbol with ASCII value in the range [64 … 96]**
- x is an **integer in the range [1… a]**
- y is an **integer in the range [1… b]**

### **Output:**

Print on the console:

- The generated code
   - If the number of combinations is larger than the maximum of the code, print to the submitted value
   - Otherwise, print to the current number of combinations

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2 | #@11@#\|$A12A$\|%B13B%\|&amp;C21C&amp;\|&#39;D22D&#39;\|(E23E(\| | Since reaching the value of numbers **a** and **b**   |
| 3 | | in advance of reaching the maximum number|
| 10 | | of combinations, the program ends.|
| 20 | #@11@#\|$A12A$\|%B13B%\|&amp;C14C&amp;\|&#39;D15D&#39;\|(E16E(\|)F17F)\|\*G18G\*\|+H19H+\|,I110I,\| | Since reaching the maximum number of combinations |
| 50 | | of earlier values of the numbers **a** and **b** , the program ends.|
| 10 | | | 

# Examples for Exam Problems

9.\* Magic Numbers

Write a program that reads a **&quot;magical&quot;** number (integer) entered by the user, and make **all** possible **6-digit numbers**, for which the **multiplication of all the digits is equal to the &quot;magic&quot; number**.

**Examples**: &quot;Magic number&quot; -> 2

- 111112 -> 1 \* 1 \* 1 \* 1 \* 1 \* 2 = 2
- 111121 -> 1 \* 1 \* 1 \* 1 \* 2 \* 1 = 2
- 111211 -> 1 \* 1 \* 1 \* 2 \* 1 \* 1 = 2
- 112111 -> 1 \* 1 \* 2 \* 1 \* 1 \* 1 = 2
- 121111 -> 1 \* 2 \* 1 \* 1 \* 1 \* 1 = 2
- 211111 -> 2 \* 1 \* 1 \* 1 \* 1 \* 1 = 2

### **Input**

The input is read from the console and it consists of a single number - **an integer in range [1 … 600000]**

### **Output**

Print on the console **all &quot;magic&quot; numbers**, separated by **space**

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 2 | 111112 111121 111211 112111 121111 211111 |
| 8 | 111118 111124 111142 111181 111214 111222 111241 111412 111421 111811 112114 112122 112141 112212 112221 112411 114112 114121 114211 118111 121114 121122 121141 121212 121221 121411 122112 122121 122211 124111 141112 141121 141211 142111 181111 211114 211122 211141 211212 211221 211411 212112 212121 212211 214111 221112 221121 221211 222111 241111 411112 411121 411211 412111 421111 811111 |
| 531441 | 999999 |


10. Password Generator

Write a program that reads two integers **_n_** and **_l_** , entered by the user, and generates in **alphabetical** order all possible **passwords** that consist of the following **5 characters** :

- Symbol 1: a digit from **1** to **_n_**
- Symbol 2: a digit from **1** to **_n_**
- Symbol 3: small letter among the first **_l_** letters of the Latin alphabet
- Symbol 4: small letter among the first **_l_** letters of the Latin alphabet
- Symbol 5: a digit from 1 to **n** , greater than the first 2 digits

### **Input**

The input is read from the console and consists of **two integers**  **n** and **_l_** in the range **[1 ... 9]**, one per line.

### **Output**

Print on the console **all passwords** in **alphabetical** order, separated by **single space**

### **Examples**

| **Input** | **Output** |
| --- | --- |
| 2 | 11aa2 11ab2 11ac2 11ad2 11ba2 11bb2 11bc2 11bd2 11ca2 11cb2 11cc2 11cd2 11da2 11db2 11dc2 11dd2 |
| 4| |

| **Input** | **Output** |
| --- | --- |
| 3 | 11aa2 11aa3 12aa3 21aa3 22aa3 |
| 1| |

| **Input** | **Output** |
| --- | --- |
| 3 | 11aa2 11aa3 11ab2 11ab3 11ba2 11ba3 11bb2 11bb3 12aa3 12ab3 12ba3 12bb3 21aa3 21ab3 21ba3 21bb3 22aa3 22ab3 22ba3 22bb3 |
| 2| |

| **Input** | **Output** |
| --- | --- |
| 4 | 11aa2 11aa3 11aa4 11ab2 11ab3 11ab4 11ba2 11ba3 11ba4 11bb2 11bb3 11bb4 12aa3 12aa4 12ab3 12ab4 12ba3 12ba4 12bb3 12bb4 13aa4 13ab4 13ba4 13bb4 21aa3 21aa4 21ab3 21ab4 21ba3 21ba4 21bb3 21bb4 22aa3 22aa4 22ab3 22ab4 22ba3 22ba4 22bb3 22bb4 23aa4 23ab4 23ba4 23bb4 31aa4 31ab4 31ba4 31bb4 32aa4 32ab4 32ba4 32bb4 33aa4 33ab4 33ba4 33bb4 |
| 2| |