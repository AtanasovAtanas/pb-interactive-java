[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Number Sequence
[code-task title="Number Sequence" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **n** representing the count of numbers to read next
* Finds the **max** and the **min** numbers
* Prints them on the console

[/task-description]
[tests]
[test]
[input]
3
1
2
3
[/input]
[output]
Max number: 3
Min number: 1
[/output]
[/test]
[test]
[input]
2
7
1
[/input]
[output]
Max number: 7
Min number: 1
[/output]
[/test]
[test]
[input]
4
0
-1
2
3
[/input]
[output]
Max number: 3
Min number: -1
[/output]
[/test]
[test]
[input]
3
-13
-12
-9
[/input]
[output]
Max number: -9
Min number: -13
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5|Max number: 304|
|10|Min number: 0|
|20||
|304||
|0||
|50||
[/slide]

[slide]
# Problem: Power of Number
[code-task title="Power of Number" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **p** - the power and **n** - the number
* Prints the result of **n** powered by **p**

Don't use **Math.pow()**

[/task-description]
[tests]
[test]
[input]
3
2
[/input]
[output]
8
[/output]
[/test]
[test]
[input]
2
7
[/input]
[output]
49
[/output]
[/test]
[test]
[input]
4
3
[/input]
[output]
81
[/output]
[/test]
[test]
[input]
2
5
[/input]
[output]
25
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5|32|
|2||

|Input|Output|
|-----|------|
|4|81|
|3||
[/slide]

[slide]
# Problem: Biggest Number
[code-task title="Biggest Number" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **n** - number representing **amount** of input numbers
* Reads **n** numbers
* Finds and prints the **biggest** number

[/task-description]
[tests]
[test]
[input]
3
1
2
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
2
4
3
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
3
-7
-7
8
[/input]
[output]
8
[/output]
[/test]
[test]
[input]
2
5
10
[/input]
[output]
10
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|3|90|
|40||
|90||
|50||

|Input|Output|
|-----|------|
|3|-40|
|-40||
|-90||
|-50||
[/slide]

[slide]
# Problem: Equal Pairs
[code-task title="Equal Pairs" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
Reads number **n** and **n** pairs of numbers

If the sum of all pairs is the same, prints: 

"Yes, value = \{sum\}"

Otherwise, prints: 

"No, maxdiff = \{diff\}"

* **diff** is the max difference in the sum between two pairs

[/task-description]
[tests]
[test]
[input]
2
1
2
3
4
[/input]
[output]
No, maxdiff = 4
[/output]
[/test]
[test]
[input]
2
2
2
2
2
[/input]
[output]
Yes, value = 4
[/output]
[/test]
[test]
[input]
1
3
4
[/input]
[output]
Yes, value = 7
[/output]
[/test]
[test]
[input]
4
-3
0
9
10
4
3
2
1
[/input]
[output]
No, maxdiff = 22
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|Yes, value=-1|
|-1||
|0||
|-1||

[/slide]

[slide]
# Problem: Zig Zag Sum
[code-task title="Zig Zag Sum" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
Reads **n** - number representing the amount of input numbers
Reads **n** numbers: 
* For every **even** line **adds** the number to the result
* For every **odd** line **subtracts** the number from the result

Prints the result

[/task-description]
[tests]
[test]
[input]
3
1
2
3
[/input]
[output]
-2
[/output]
[/test]
[test]
[input]
3
4
5
6
[/input]
[output]
-5
[/output]
[/test]
[test]
[input]
4
-2
3
-6
4
[/input]
[output]
15
[/output]
[/test]
[test]
[input]
4
-3
0
9
10
[/input]
[output]
4
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|-30|
|10||
|-20||

[/slide]

[slide]
# Problem: Divide Without Remainder
[code-task title="Divide Without Remainder" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **n** and **n** numbers
* Finds in **percentage** how many of them can divide without remainder at **2**, **3** and **4**
* Prints percentages **p1**, **p2** and **p3**, formatted to the second digit

[/task-description]
[tests]
[test]
[input]
3
1
2
3
[/input]
[output]
33.33
33.33
0.00
[/output]
[/test]
[test]
[input]
3
4
5
6
[/input]
[output]
66.67
33.33
33.33
[/output]
[/test]
[test]
[input]
4
-2
3
-6
4
[/input]
[output]
75.00
50.00
25.00
[/output]
[/test]
[test]
[input]
4
-3
0
9
10
[/input]
[output]
50.00
75.00
25.00
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|3|33.33|
|3|100.00|
|6|0.00|
|9||

|Input|Output|
|-----|------|
|3|66.67|
|4|66.67|
|6|33.33|
|3||

[/slide]

[slide]
# Problem: Vowel Sum
[code-task title="Vowel Sum" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads n - the count of characters:
* Adds a character’s value to the result if it is a vowel

|**character**|**a**|**e**|**i**|**o**|**u**|
|-------------|-----|-----|-----|-----|-----|
|value|1|2|3|4|5|

* Prints the result

[/task-description]
[tests]
[test]
[input]
3
a
v
d
[/input]
[output]
1
[/output]
[/test]
[test]
[input]
4
a
u
r
t
[/input]
[output]
6
[/output]
[/test]
[test]
[input]
3
a
e
r
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
2
e
o
[/input]
[output]
6
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|1|
|a||
|g||

|Input|Output|
|-----|------|
|2|8|
|i||
|u||

[/slide]

[slide]
# Problem: Rollercoaster
[code-task title="Rollercoaster" taskId="p-08" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **rollercoaster places**, **minimum age**, **count of people** on the queue and **age** for each person
* Prints "**The rollercoaster departures**" if all places are taken
* Prints "**Waiting**" in all other cases

[/task-description]
[tests]
[test]
[input]
5
10
3
1
2
3
[/input]
[output]
Waiting
[/output]
[/test]
[test]
[input]
4
3
2
1
4
[/input]
[output]
Waiting
[/output]
[/test]
[test]
[input]
5
10
3
20
5
5
[/input]
[output]
Waiting
[/output]
[/test]
[test]
[input]
3
4
5
6
7
8
9
6
[/input]
[output]
The rollercoaster departures
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|1|The rollercoaster departures|
|10||
|1||
|15||

[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" taskId="p-09" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]

Write a program, which: 
* Reads **n** - an integer from the console
* Prints **n**'s first multiples in the format 

"\{n\} x \{i\} = \{result\}"

[/task-description]
[tests]
[test]
[input]
3
[/input]
[output]
3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
3 x 4 = 12
3 x 5 = 15
3 x 6 = 18
3 x 7 = 21
3 x 8 = 24
3 x 9 = 27
3 x 10 = 30
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|2 x 1 = 2|
||2 x 2 = 4|
||2 x 3 = 4|
||2 x 4 = 4|
||2 x 5 = 4|
||...|
||2 x 10 = 20|
[/slide]