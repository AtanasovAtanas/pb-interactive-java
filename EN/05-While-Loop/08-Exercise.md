## **Exercise: While Loop**

1. Sequence 2k+1

Write a program that reads a number **n** and prints **all numbers ≤ n** from the sequance: **1, 3, 7, 15, 31** ,… Every next number is calculated as you **multiply the previous number by 2 and add 1**.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 3 | 1 | | 8 | 1 | | 17 | 1 | | 31 | 1 |
|  | 3 | | | 3 | | | 3 | | | 3 |
| | | | | 7 | | | 7 | | | 7 |
| | | | | | | | 15 | | | 15 |
| | | | | | | | | | | 31 |

2. Max Number

Write a program that takes as input **n count integers (n > 0)** and finds the **max** among them. First you read the count of numbers **n**, and after that the **numbers** - each on a **single** line.

### **Examples**

| **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |   | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | 100 | | 3 | 20 | | 4 | 99 | | 1 | 999 | | 2 | -1 |
| 100 | | | -10 | | | 45 | | | 999 | | | -1 | |
| 99 | | | 20 | | | -20 | | | | | | -2 | |
| | | | -30  | | | 7 | | | | | | | |
| | | | | | | | | | | | | | |

3. Graduation

Write a program that calculates the **average grade** of a student from his entire education. On the first line you will receive **the name of the student**, and oneach following line his annual grades. The student passes to upper class, if his **annual grade is 4.00 or greater**. If his grade is less than 4.00, he has to **repeat** the class.

If the student graduates **12th** class, you have to print:

**&quot;{student name} graduated. Average grade: {average grade from his entire education}&quot;**

**The grade should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | | **Input** | **Output** | | **Input** | **Output** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| John | John graduated. Average grade: 5.37 | | Mike | Mike graduated. Average grade: 5.25 | | Ani | Ani graduated. Average grade: 5.45 |
| 4 | | | 5 | | | 5 | | |
| 5.5 | | | 5 | | | 5.32| | |
| 6 | | | 5 | | | 6 | | |
| 5.43 | | | 6 | | | 5.43 | | |
| 4.5 | | | 5.5 | | | 5 | | |
| 6 | | | 5 | | | 6 | | |
| 5.55 | | | 6 | | | 5.5 | | |
| 5 | | | 5.44 | | | 4.55 | | |
| 6 | | | 5 | | | 5 | | |
| 6 | | | 5 | | | 6 | | |
| 5.43 | | | 5 | | | 5.56 | | |
| 5 | | | 5 | | | 6 | | |
| | | | 6 | | | | | |
| | | | 5.45 | | | | | |

4. Old Books

Ani goes to her home town after being a long time abroad. When she comes home, she sees her grandmother&#39;s library and remembers her favourite book. Help Ani writing a program in which Ani enters the name of the **book** she&#39;s searching for (**String**) and the **capacity** of the library (**integer**). **Until Ani finds her favourite book or doesn&#39;t check all books in the library, the program have to reads every time the name of the next book on a separate line.**

- If Ani **doesn&#39;t** find the book, print **two** lines:

  - **&quot;The book you search is not here!&quot;**
  - **&quot;You checked {count} books.&quot;**

- If Ani **finds** the book, print a **single** line:
  - **&quot;You checked {count} books and found it.&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| Troy | You checked 2 books and found it. | In that case the book Ani is searching for is Troy, and the library&#39;s capacity is 8 books.  |
| 8 | | The first book is Stronger, the second one is Life Style, the third one is desired - Troy and the program ends.|
| Stronger | | |
| Life Style | | |
| Troy | | |


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| The Spot | The book you search is not here! | The book Ani is searching for is &quot;The Spot&quot;. The library contains 4books.  |
| 4 | You checked 4 books. | The first book is Hunger Games, the second - Harry Potter, the third - Torronto, the fourth - Spotify.|
| Hunger Games | | Since there aren&#39;t other books in the library, reading names is stopped. Ani didn&#39;t find the book.|
| Harry Potter | | |
| Torronto | | |
| Spotify | | |


| **Input** | **Output** |
| --- | --- |
| Bourne| You checked 10 books and found it. |
| 32| |
| True Story| |
| Forever| |
| More Space| |
| The Girl| |
| Spaceship| |
| Strongest| |
| Profit| |
| Tripple| |
| Stella| |
| The Matrix| |
| Bourne| |

5. Exam Preparation

Write a program in which Martin solves problems for exams until he receives message from his lecturer: **&quot;Enough&quot;**. Every time he solves a problem, he get a grade. **The program should ends either Martin receives &quot;Enough&quot; command, or obtain the number of poor grades. A poor grade is a grade less or equal to 4.00.**

### **Input**

- On the first line – **number of poor grades** – **integer in range [1…5]**
- **After that repeatedly two lines**** :**

  - **Name of a problem - text**

  - **Grade - integer in range [2…6]**

### **Output**

- If Martinreaches **&quot;Enough&quot;** command, print **3** lines:

  - **&quot;Average score: {average grade}&quot;**
  - **&quot;Number of problems: {number of ALL problems}&quot;**
  - **&quot;Last problem: {**** last problem&#39;s name ****}&quot;**

- **If he gets the specified number of poor grades**:

  - **&quot;You need a break, {number poor grades} poor grades.&quot;**

**The average grade should be formatted to the second decimal point.**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 3 | Average score: 5.25 | The number of allowed poor grades is 3.|
| Money | Number of problems: 4 | First problem&#39;s name is Money, Martin&#39;s grade is 6.|
| 6 | Last problem: Bus |  Second problem - Story, grade - 4.|
| Story | | Third problem - Spring Time, grade - 5.|
| 4 | | Fourth problem - Bus, grade - 6.|
| Spring Time | | Next command is Enough, the program ends.|
| 5 | |  Average grade: 21 / 4 = 5.25|
| Bus | | Number of solved problems: 4|
| 6 | | Last problem: Bus|
| Enough | | |


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 2| You need a break, 2 poor grades. | The number of allowed poor grades is 2.  |
| Income| | The first problem&#39;s name is Income, Martin&#39; grade is 3.|
| 3| | Second problem - Game Info, grade - 6.|
| Game Info| | Third problem - Best Player, grade - 4.|
| 6| | Martin reaches the number of allowed poor grades, it is time for break.|
| Best Player| | |
| 4| | |

6. Walking

Gaby wants to start healthy life and shesets a goal to walk **10 000 steps** a **day**. Although, some days Gaby is so tired she wants to go home before she reaches the goal. Write a program **that reads from the console how many steps** Gaby walks every time she is out and **when she reaches the set goal**, print a message **&quot;Goal reached! Good job!&quot;**.

In case she wants to go home **before** reaching the goal, she will enter **&quot;Going home&quot;** command and the **steps** she had **walked** while she was **going home**. After that, if she didn&#39;t manage to reach her goal, you have to print the following massage on the console: **&quot;{difference in steps} more steps to reach goal.&quot;**

### **Examples**

| **Input** | **Output** | | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 1000 | Goal reached! Good job! | | 1500 | 2500 more steps to reach goal. |
| 1500| | | 300| |
| 2000| | | 2500| |
| 6500| | | 3000| |
| | | | Going home| |
| | | | 200| |


| **Input** | **Output** | | **Input** | **Output** |
| --- | --- | --- | --- | --- |
| 1500 | Goal reached! Good job! | | 125 | Goal reached! Good job! |
| 3000| | | 250| |
| 250| | | 4000| |
| 1548| | | 30| |
| 2000| | | 2678| |
| Going home| | | 4682| |
| 2000| | | | |

7. Stream Of Letters

Write a program that reads a hidden message in a sequence of symbols. You will receive each of them on a single line until the **&quot;End&quot;** command. The words are initiated from the letters in the **order of their reading**. Symbols which are **not Latin** letters should be **ignored**. The words, hidden in the stream, are separated from a **secret command by three letters** - **&quot;c&quot;**, **&quot;o&quot;** and **&quot;n&quot;**. When you **first receive** one of these letters, you have to mark it as visited, **but it is not saved in the word**. Every time you **receive the same** letter, **it is saved normally** in the word. After you have found **all three symbols from the command**, you have to print the word and a space &quot; &quot;. A new word is started at the same way, waiting the secret command to be printed.

### **Input**

Read a sequence of lines with a single symbol each, until you receive the **&quot;End&quot;** command

### **Output**

Print on the console **every word after the secret command** followed by **space**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| H | Hello there | **&quot;H&quot;**, **&quot;n&quot;**, **&quot;e&quot;**, **&quot;l&quot;**, **&quot;l&quot;**, **&quot;o&quot;**, **&quot;o&quot;**, **&quot;c&quot;**, **&quot;t&quot;**, **&quot;c&quot;**, **&quot;h&quot;**, **&quot;o&quot;**, **&quot;e&quot;**, **&quot;r&quot;**, **&quot;e&quot;**, **&quot;n&quot;**, **&quot;e&quot;** are all read letters.|
| n| | First we read **&quot;H&quot;** and we add it to the word. The next symbol is **&quot;n&quot;**. It&#39;s part of the command and we **do not add it to the word as we meet it for the first time**.|
| e| | The next symbols are **&quot;e&quot;**, **&quot;l&quot;**, **&quot;l&quot;** and we add them to the word. We read **&quot;o&quot;** and we mark it as visited,|
| l| | but again we do **not** add it to the word. The next letter is **&quot;o&quot;** again and it&#39;s added. The next is **&quot;c&quot;** and all three symbols for the secret command are available.|
| l| | We **print &quot;Hello &quot;** and we watch for new secret command. We read **&quot;t&quot;** and we add it to the new word.|
| o| | After that the **&quot;c&quot;** is part of the new command and we do **not** add it.|
| o| | We read **&quot;h&quot;** and add it to the word. Next is **&quot;o&quot;** which is part of the new command. We read **&quot;e&quot;**, **&quot;r&quot;**, **&quot;e&quot;** and add them to the word.|
| c| | Next is **&quot;n&quot;** and the secret command is done. We print **&quot;there &quot;**. The next read symbol is **&quot;e&quot;** and it&#39;s added to a new word.|
| t| | We receive the **&quot;End&quot;** command and the program ends.The final result is **&quot;Hello there &quot;.**|
| c| | |
| h| | |
| o| | |
| e| | |
| r| | |
| e| | |
| n| | |
| e| | |
| End| | |


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| % | BooM | **&quot;%&quot;**, **&quot;!&quot;**, **&quot;c&quot;**, **&quot;^&quot;**, **&quot;B&quot;**, **&quot;\`&quot;**, **&quot;o&quot;**, **&quot;%&quot;**, **&quot;o&quot;**, **&quot;o&quot;**, **&quot;M&quot;** , **&quot;)&quot;**, **&quot;{&quot;**, **&quot;n&quot;**, **&quot;\\&quot;**, **&quot;A&quot;**, **&quot;D&quot;** are all symbols from the console.|
| !| | We skip **&quot;%&quot;** and **&quot;!&quot;**, because they are **not part of the Latin alphabet**.|
| c| | We read **&quot;c&quot;** and save it for the secret command **without add it to the word**. We skip **&quot;^&quot;**. Next is **&quot;B&quot;** and is added to the word.|
| ^| | **&quot;\`&quot;** is skipped. Next is **&quot;o&quot** – part of the secret command and it&#39;s **NOT** added to the word. We skip **&quot;%&quot;**.|
| B| | The next symbols are **&quot;o&quot;**, **&quot;o&quot;**, **&quot;M&quot;** and we add them one by one to the word. We skip **&quot;)&quot;** and **&quot;{&quot;**.|
| \`| | Next is **&quot;n&quot** and the secret command is finished. We print **&quot;BooM &quot;**. We skip **&quot;\\&quot;**.|
| o| | The next are **&quot;A&quot;**, **&quot;D&quot** and add them to a new word. We read the **&quot;End&quot;** command and the program ends.|
| %| | The final result is **&quot;BooM &quot;**.|
| o| | |
| o| | |
| M| | |
| )| | |
| {| | |
| n| | |
| \\| | |
| A| | |
| D| | |
| End| | |


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| o | Solve me | **&quot;o&quot;**, **&quot;S&quot;**, **&quot;%&quot;**, **&quot;o&quot;**, **&quot;l&quot;**, **&quot;^&quot;**, **&quot;v&quot;**, **&quot;e&quot;**, **&quot;c&quot;**, **&quot;n&quot;**, **&quot;&&quot;**, **&quot;m&quot;**, **&quot;e&quot;**, **&quot;c&quot;**, **&quot;o&quot;** and **&quot;n&quot;** are all the symbols we read from the console. |
| S| | First we read **&quot;o&quot;** and we keep it in the secret command, **without adding it to the word**. Next is **&quot;S&quot;** and we add it to the word.|
| %| | We skip  **&quot;%&quot;**. Next are **&quot;o&quot;** and **&quot;l&quot;** and are added to the word. We skip **&quot;^&quot;**.|
| o| | Next are **&quot;v&quot;** and **&quot;e&quot;** and we add them to the word. We read **&quot;c&quot;** and **&quot;n&quot;** and the command is finished.|
| l| | We print **&quot;Solve &quot;**. **&quot;&&quot;** is skipped. **&quot;m&quot;** and **&quot;e&quot;** are added to a new word.|
| ^| | Next are **&quot;c&quot;**, **&quot;o&quot;** and **&quot;n&quot;** and the command is ready. We print **&quot;me &quot;**.|
| v| | The **&quot;End&quot;** command is next and the program ends. The final result is **&quot;Solve me &quot;**.|
| e| | |
| c| | |
| n| | |
| &| | |
| m| | |
| e| | |
| c| | |
| o| | |
| n| | |
| End| | |

## **Examples for Exam Problems**

8. \* Cake

You&#39;ve been invited to 30th Birthday and the birthday boy istreating with a huge cake. However, he doesn&#39;t know **how many pieces the guests could take**. Your task is to write a program that calculates **how many pieces** the guest took before the cake is over. You will receive the **dimensions of the cake in centimeters** (width and length - **integers** in range [1…1000]) and after that on every line until you receive **&quot;STOP&quot;** command or **until there are no more pieces of the cake**. The pieces are in shape of **square** with size 1 cm.

**Print** on the console **one** of the following lines:

- **&quot;{number of pieces} pieces are left.&quot;** - if you reach the **STOP** command and there are pieces left

- **&quot;No more cake left! You need {number of needed pieces} pieces more.&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 10 | No more cake left! You need 1 pieces more. | The cake is with length **10** and width **10** |
| 10| | => number of pieces = **10** \* **10** = **100**|
| 20| | 1-st fraction -> 100 - 20 = 80|
| 20| | 2-nd fraction -> 80 - 20 = 60|
| 20| | 3-rd fraction -> 60 - 20 = 40|
| 20| | 4-th fraction -> 40 - 20 = 20|
| 21| | 5-th fraction -> 20 - 21 = -1 < 0|
| | | => there are no more pieces, 1 piece is needed|


| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 10 | 8 pieces are left. | The cake is with length **10** and width **2** |
| 2| | => number of pieces = **10** \* 2 = 20|
| 2| | 1-st fraction -> 20 - 2 = 18|
| 4| | 2-nd fraction -> 18 - 4 = 14|
| 6| | 3-rd fraction -> 14 - 6 = 8|
| STOP| | 4-th fraction -> command STOP|
| | | => left pieces: 8|

9. \* Moving

On his 18th Birthday John made a decision to move out and to live in accommodation. He packed his luggage in **boxes** and found suitable advertisement for apartment. He starts to move his luggage on **partitions**, because he can&#39;t move it at once. There is **limited free space** in his new apartment where he can put his stuffs.

Write a program for calculating the **free volume** of John&#39;s house **after he moves out**.

**Note: A box has exact dimensions:  1m. x 1m. x 1m.**

### **Input**

The user enters the following **data** on **separate** lines:

1. **Width** of the free space - **integer in range [1...1000]**
2. **Length** of the free space - **integer in range [1...1000]**
3. **Height** of the free space - **integer in range [1...1000]**
4. On the next few lines **(until the &quot;Done&quot; command is recieved) - number of boxes that are moving in the apartment - integers in range [1...10000]**

**The program should ends reading input either when the &quot;Done&quot; command is received, or there is no more free space.**

### **Output**

**Print** on the console **one** of the following lines:

- If you reach the **&quot;Done&quot;** command and there **IS** more free space:
**&quot;{amount of free m<sup>3</sup>} Cubic meters left.&quot;**

- If the free space overs before you reach the **&quot;Done&quot;** command:
**&quot;No more free space! You need {amount m<sup>3</sup> needed} Cubic meters more.&quot;**

### **Examples**

| **Input** | **Output** | **Comments** |
| --- | --- | --- |
| 10| No more free space! You need 2 Cubic meters more.| 10 * 10 * 2 = **200 m<sup>3</sup>**|
| 10| | 20 + 20 + 20 + 20 + 122 = **202 m<sup>3</sup>**|
| 2| | 200 - 202 = **2 m<sup>3</sup> needed**|
| 20| | |
| 20| | |
| 20| | |
| 20| | |
| 122| | |