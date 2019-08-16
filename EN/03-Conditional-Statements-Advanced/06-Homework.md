[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[tests]
[test]
[input]
kiwi
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
carrot
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
pepper
[/input]
[output]
vegetable
[/output]
[/test]
[test]
[input]
fruit
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Problem: Day of Week
[code-task title="Day of Week" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[tests]
[test]
[input]
1
[/input]
[output]
Monday
[/output]
[/test]
[test]
[input]
12
[/input]
[output]
Error
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
Wednesday
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
Friday
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Problem: Vowel or Consonant
[code-task title="Vowel or Consonant" taskId="p-03" executionType="tests-execution"  executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[tests]
[test]
[input]
e
[/input]
[output]
Vowel
[/output]
[/test]
[test]
[input]
i
[/input]
[output]
Vowel
[/output]
[/test]
[test]
[input]
h
[/input]
[output]
Consonant
[/output]
[/test]
[test]
[input]
t
[/input]
[output]
Consonant
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Problem: Product of 3 Numbers
[code-task title="Product of 3 Numbers" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[tests]
[test]
[input]
2.5
4.5
3.5
[/input]
[output]
positive
[/output]
[/test]
[test]
[input]
-9.6
9.1
0.5
[/input]
[output]
negative
[/output]
[/test]
[test]
[input]
0
0
0
[/input]
[output]
zero
[/output]
[/test]
[test]
[input]
-4.5
-0.1
-9.1
[/input]
[output]
negative
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Problem: Sorted Numbers
[code-task title="Sorted Numbers" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[tests]
[test]
[input]
2.5
4.5
3.5
[/input]
[output]
not sorted
[/output]
[/test]
[test]
[input]
1.2
1.3
1.4
[/input]
[output]
Ascending
[/output]
[/test]
[test]
[input]
-1.5
-1.4
-1.3
[/input]
[output]
Ascending
[/output]
[/test]
[test]
[input]
3.5
3.4
3.2
[/input]
[output]
Descending
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[tests]
[test]
[input]
Spring
Hotel
4
[/input]
[output]
96.00
[/output]
[/test]
[test]
[input]
Summer
Camping
5
[/input]
[output]
150.00
[/output]
[/test]
[test]
[input]
Winter
Hotel
3
[/input]
[output]
108.00
[/output]
[/test]
[test]
[input]
Autumn
Camping
10
[/input]
[output]
105.00
[/output]
[/test]
[/tests]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]


[slide]
# Problem: Cinema
[code-task title="Cinema" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[tests]
[test]
[input]
Premiere
1
2
[/input]
[output]
24.00
[/output]
[/test]
[test]
[input]
Normal
3
5
[/input]
[output]
112.50
[/output]
[/test]
[test]
[input]
Discount
7
6
[/input]
[output]
210.00
[/output]
[/test]
[test]
[input]
Normal
3
4
[/input]
[output]
90.00
[/output]
[/test]
[/tests]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal|810.00|
|12||
|9||
[/slide]


[slide]
# Problem: Operations with Numbers
[code-task title="Operations with Numbers" taskId="p-08" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to apply an operator for given two numbers:

* Read two real numbers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[tests]
[test]
[input]
1
2
+
[/input]
[output]
1 + 2 = 3
[/output]
[/test]
[test]
[input]
5
3
-
[/input]
[output]
5 - 3 = 2
[/output]
[/test]
[test]
[input]
3
5
*
[/input]
[output]
3 * 5 = 15
[/output]
[/test]
[test]
[input]
10
2
/
[/input]
[output]
10 / 2 = 5
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|12||
|+||
[/slide]


[slide]
# Problem: ATM
[code-task title="ATM" taskId="p-09" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[tests]
[test]
[input]
100
30
40
[/input]
[output]
The withdraw was successful.
[/output]
[/test]
[test]
[input]
30
300
200
[/input]
[output]
The daily limit was exceeded.
[/output]
[/test]
[test]
[input]
150
30
200
[/input]
[output]
The withdraw was successful.
[/output]
[/test]
[test]
[input]
10
2
/
[/input]
[output]
10 / 2 = 5
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420|The withdraw was successful.|
|20||
|25||
|10|The daily limit was exceeded.|
|50|Insufficient availability.|
|20||
[/slide]

[slide]
# Problem: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" taskId="p-10" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[tests]
[test]
[input]
1
2
3
4
5
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
0
-1
-3
4
10
[/input]
[output]
10
[/output]
[/test]
[test]
[input]
-1
-2
-3
-4
-5
[/input]
[output]
-1
[/output]
[/test]
[test]
[input]
10
2
20
30
2
[/input]
[output]
30
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]

[slide]
# Video

[vimeo-video videoId="341582556" startTimeInSeconds="7275" endTimeInSeconds="11375" /]

[/slide]