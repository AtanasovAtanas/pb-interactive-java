[slide]
# Homework
Welcome to the homework. 

Now we are going to write a couple of console applications, by which we are going to make a few more steps into programming. 

We have prepared some problems for you to solve.

Let's solve a few problems to confirm what we have learned.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/homeowrk.png"/]
[/slide]


[slide]
# Problem: Biggest Number
[code-task title="Biggest Number" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads **n** - number representing amount of input numbers
* Reads n numbers
* Finds and prints the **biggest number**
# Example
## Input
- 3
- 40
- 90
- 50
## Output
- 90
[/task-description]
[tests]
[test]
[input]
3
30
80
40
[/input]
[output]
80
[/output]
[/test]
[test]
[input]
3
-30
-80
-40
[/input]
[output]
-30
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Biggest Number
[code-task title="Biggest Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        int maxNumber = Integer.MIN_VALUE;
        for (int i = 1; i <= n; i++) {
            int number =
                    Integer.parseInt(sc.nextLine());
            if (number > maxNumber) {
                maxNumber = number;
            }
        }
        System.out.println(maxNumber);
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
[code-io /]
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
# Problem: Number Sequence
[code-task title="Number Sequence" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads **n** representing the count of numbers to read next
* Finds the **max** and the **min numbers**
* Prints them on the console
# Example
## Input
- 5
- 10
- 304
- 0
- 0
- 50
## Output
- Max number: 304
- Min number: 0
[/task-description]
[tests]
[test]
[input]
4
100
200
0
300
[/input]
[output]
Max number: 300
Min number: 0
[/output]
[/test]
[test]
[input]
1
100
[/input]
[output]
Max number: 100
Min number: 100
[/output]
[/test]
[test]
[input]
3
-1
-2
0
[/input]
[output]
Max number: 0
Min number: -2
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Number Sequence
[code-task title="Number Sequence" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        int min = Integer.MAX_VALUE;
        int max = Integer.MIN_VALUE;
        for (int i = 0; i < n; i++)
        {
            int num = Integer.parseInt(sc.nextLine());

            if (num < min) min = num;
            if (num > max) max = num;
        }
        System.out.printf("Max number: %d%n", max);
        System.out.printf("Min number: %d%n", min);
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
[code-io /]
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
[code-task title="Power of Number" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads **p – the power** and **n – the number**
* Prints the result of n powered by p
* Don't use Math.Pow()
# Example
## Input
- 5
- 2
## Output
- 32
[/task-description]
[tests]
[test]
[input]
5
2
[/input]
[output]
32
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Power of Number
[code-task title="Power of Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int p = Integer.parseInt(sc.nextLine());
        int n = Integer.parseInt(sc.nextLine());
        int result = 1;
        for(int i = 0; i < p; i++)
        {
            result = result * n;
        }
        System.out.println(result);
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
[code-io /]
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
# Description
Write a program, which:

* Reads number **n** and **n pairs** of numbers
* Prints "Yes, value=\{sum\}", if the **sum of all** pairs is the **same**
* **Otherwise**, prints "No, maxdiff=\{diff\}"
* diff is the **max difference** in the sum between two pairs
# Example
## Input
- 2
- -1
- 0
- 0
- -1
## Output
- Yes, value=-1
[/task-description]
[tests]
[test]
[input]
3
1
2
0
3
4
-1
[/input]
[output]
Yes, value=3
[/output]
[/test]
[test]
[input]
2
1
2
2
2
[/input]
[output]
No, maxdiff=1
[/output]
[/test]
[test]
[input]
4
1
1
3
1
2
2
0
0
[/input]
[output]
No, maxdiff=4
[/output]
[/test]
[test]
[input]
1
5
5
[/input]
[output]
Yes, value=10
[/output]
[/test]
[test]
[input]
2
-1
0
0
-1
[/input]
[output]
Yes, value=-1
[/output]
[/test]
[test]
[input]
2
-1
2
0
-1
[/input]
[output]
No, maxdiff=2
[/output]
[/test]
[test]
[input]
8
5
5
70
-60
3
7
2
8
20
-10
15
-5
0
10
10
0
[/input]
[output]
Yes, value=10
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Equal Pairs
[code-task title="Equal Pairs" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        int prevSum = 0;
        int maxDiff = 0;
        boolean areEqual = true;
        for (int i = 0; i < n; i++) {
            int a = Integer.parseInt(sc.nextLine());
            int b = Integer.parseInt(sc.nextLine());
            if (i > 0) {
                if (maxDiff < Math.abs(prevSum - a - b))
                    maxDiff = Math.abs(prevSum - a - b);
                if (areEqual && a + b != prevSum)
                    areEqual = false;
            }
            prevSum = a + b;
        }
        if (areEqual){
            System.out.printf("Yes, value= %d",prevSum);
        }else{
            System.out.printf("No, maxdiff= %d",maxDiff);
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
Reads number **n** and **n** pairs of numbers
Prints "**Yes, value=\{sum\}**", if the sum of all pairs is the same
Otherwise, prints "**No, maxdiff=\{diff\}**"
* **diff** is the max difference in the sum between two pairs

[/task-description]
[code-io /]
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
# Description
Write a program, which:

* Reads **n** - number representing amount of input numbers
* Reads **n numbers** 
* For every **even** line **adds** the number to the result
* For every **odd** line **subtracts** the number from the result
* **Prints** the result
# Example
## Input
- 2
- 10
- 20
## Output
- 10
[/task-description]
[tests]
[test]
[input]
4
20
20
20
20
[/input]
[output]
0
[/output]
[/test]
[test]
[input]
2
10
20
[/input]
[output]
10
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]

[/slide]

[slide]
# Solution: Zig Zag Sum
[code-task title="Zig Zag Sum" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        int sum = 0;
        for (int i = 1; i <= n; i++) {
            int m = Integer.parseInt(sc.nextLine());
            if (i % 2 == 0) sum += m;
            else sum -= m;
        }
        System.out.println(sum);
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
[code-io /]
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
# Description
Write a program, which:

* Reads **n** and **n numbers**
* Finds in **percentage** how many of them can **divide without remainder** at **2**, **3** and **4**
* Prints percentages p1, p2 and p3, **formatted** to the second digit
# Example
## Input
- 3
- 3
- 6
- 9
## Output
- 33.33%
- 100.00%
- 0.00%
[/task-description]
[tests]
[test]
[input]
3
12
27
6
[/input]
[output]
66.67%
100.00%
33.33%
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Divide Without Remainder
[code-task title="Divide Without Remainder" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        double p1 = 0.0;
        double p2 = 0.0;
        double p3 = 0.0;
        for (int i = 0; i < n; i++) {
            int num = Integer.parseInt(sc.nextLine());
            if (num % 2 == 0) {
                p1++;
            }
            if (num % 3 == 0) {
                p2++;
            }
            if (num % 4 == 0) {
                p3++;
            }
        }
        double resultP1 = (p1 / n) * 100;
        double resultP2 = (p2 / n) * 100;
        double resultP3 = (p3 / n) * 100;

        System.out.printf("%.2f%n", resultP1);
        System.out.printf("%.2f%n", resultP2);
        System.out.printf("%.2f%n", resultP3);

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
[code-io /]
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
# Description
Write a program, which:

* Reads **n** - the count of characters:
* If character is **vowel** adds its value to the result

    |character|a|e|i|o|u|
    |---------|-|-|-|-|-|
    |value|1|2|3|4|5|

* Prints the result
# Example
## Input
- 2
- a
- g
## Output
- 1
[/task-description]
[tests]
[test]
[input]
2
i
u
[/input]
[output]
8
[/output]
[/test]
[test]
[input]
5
a
u
n
m
s
[/input]
[output]
6
[/output]
[/test]
[test]
[input]
1
a
[/input]
[output]
1
[/output]
[/test]
[test]
[input]
8
a
e
i
o
u
a
a
s
[/input]
[output]
17
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Vowel Sum
[code-task title="Vowel Sum" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());
        int vowelSum = 0;
        for (int i = 0; i < n; i++) {
            char letter = sc.nextLine().charAt(0);
            switch (letter) {
                case 'a': vowelSum += 1; break;
                case 'e': vowelSum += 2; break;
                case 'i': vowelSum += 3; break;
                case 'o': vowelSum += 4; break;
                case 'u': vowelSum += 5; break;
            }
        }
        System.out.println(vowelSum);
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
[code-io /]
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
# Description
Write a program, which:

* Reads rollercoaster **places**, **minimum age**, **count of people** on the queue and **age** for each person
* If all places are taken, prints - **"The rollercoaster departures"**
* In other case, prints **"Waiting..."**
# Example
## Input
- 2
- 10
- 2
- 15
- 24
## Output
- The rollercoaster departures
[/task-description]
[tests]
[test]
[input]
2
10
2
15
24
[/input]
[output]
The rollercoaster departures
[/output]
[/test]
[test]
[input]
2
25
5
10
15
18
5
30
[/input]
[output]
Waiting...
[/output]
[/test]
[test]
[input]
4
18
10
15
57
14
35
68
45
23
14
24
26
[/input]
[output]
The rollercoaster departures
[/output]
[/test]
[test]
[input]
3
21
5
25
45
34
12
24
[/input]
[output]
The rollercoaster departures
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Rollercoaster
[code-task title="Rollercoaster" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int places = Integer.parseInt(sc.nextLine());
        int minAge = Integer.parseInt(sc.nextLine());
        int peopleCount = Integer.parseInt(sc.nextLine());
        int validPeopleCount = 0;
        for (int i = 0; i < peopleCount; i++) {
            int personAge = Integer.parseInt(sc.nextLine());
            if (personAge >= minAge && places > validPeopleCount)
                validPeopleCount++;
        }
        if (places==validPeopleCount){
            System.out.println("The rollercoaster departures");
        }else {
            System.out.println("Waiting");
        }
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
[code-io /]
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
# Description
Write a program, which: 

* Reads **n** 
* Prints **n's multiples** in the format "\{n\} x \{i\} = \{result\}"
* Where i are the numbers from **1 to 10** (**inclusive**)

# Example
## Input
- 2
## Output
- 2 x 1 = 2
- 2 x 2 = 4
- 2 x 3 = 6
- 2 x 4 = 8
- 2 x 5 = 10
- 2 x 6 = 12
- 2 x 7 = 14
- 2 x 8 = 16
- 2 x 9 = 18
- 2 x 10 = 20
[/task-description]
[tests]
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
[/tests]
[code-io/]
[/code-task]

[/slide]