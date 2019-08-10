[slide]
# For Loop with Step
In this section we will pay attention to a particular and very important part of the `for` loop, namely the **step**.

**The step** is that **part** of the `for` loop construction that tells **how** much to **increase** or **decrease** the value of its **leading** variable. 

It is declared the last in the skeleton of the for loop.

Most often, we have **a size of** `1`, and in this case, instead of writing `i += 1` or `i -= 1`, we can use the `i++` or `i--` operators.

```java
for (int i = 0; i < 10; i++) {
  System.out.println(i);
}
```

If we want our step to be **different than 1**, when increasing, we use the `i +=` + step size operator. With step of 2, the loop would look like this:
```java
for (int i = 0; i < 10; i += 2) {
  System.out.println(i);
}
```

We might want to have a decreasing step - `i -=` + step size. In this case we should pay attention to the end condition to avoid an infinite loop.

```java
for (int i = 10; i >= 1; i--) {
  System.out.println(i);
}
```
[/slide]

[slide]
# Problem: Numbers Ending with 7 
[code-task title="Numbers Ending with 7" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads a number **n**
* Prints all numbers from **7** to **n**, ending with 7

[/task-description]
[tests]
[test]
[input]
30
[/input]
[output]
7
17
27
[/output]
[/test]
[test]
[input]
20
[/input]
[output]
7
17
[/output]
[/test]
[test]
[input]
50
[/input]
[output]
7
17
27
37
47
[/output]
[/test]
[test]
[input]
23
[/input]
[output]
7
17
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|27|7|
||17|
||27|

|Input|Output|
|-----|------|
|40|7|
||17|
||27|
||37|
[/slide]

[slide]
# Solution: Numbers Ending with 7 
[code-task title="Numbers Ending with 7" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = Integer.parseInt(scanner.nextLine());
        for (int i = 7; i <= n; i += 10) {
            System.out.println(i);
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads a number **n**
* Prints all numbers from **7** to **n**, ending with 7

[/task-description]
[tests]
[test]
[input]
30
[/input]
[output]
7
17
27
[/output]
[/test]
[test]
[input]
20
[/input]
[output]
7
17
[/output]
[/test]
[test]
[input]
50
[/input]
[output]
7
17
27
37
47
[/output]
[/test]
[test]
[input]
23
[/input]
[output]
7
17
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|27|7|
||17|
||27|

|Input|Output|
|-----|------|
|40|7|
||17|
||27|
||37|
[/slide]

[slide]
# Problem: Exam Countdown
[code-task title="Exam Countdown" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads an **integer** - count of days before an exam
* For each day prints: 

"\{currentDay\} days before the exam"
* At the end prints: 

"The exam has come"


[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
4 days before the exam
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
5 days before the exam
4 days before the exam
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam|
||2 days before the exam|
||1 days before the exam|
||The exam has come|
[/slide]

[slide]
# Solution: Exam Countdown
[code-task title="Exam Countdown" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int days = Integer.parseInt(scanner.nextLine());
        for (int i = days; i >= 1; i -= 1) {
            System.out.printf("%d days before the exam%n", i);
        }
        System.out.println("The exam has come");
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads an **integer** - count of days before an exam
* For each day prints: 

"\{currentDay\} days before the exam"
* At the end prints: 

"The exam has come"

[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
4 days before the exam
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
5 days before the exam
4 days before the exam
3 days before the exam
2 days before the exam
1 days before the exam
The exam has come
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|3|3 days before the exam|
||2 days before the exam|
||1 days before the exam|
||The exam has come|
[/slide]

[slide]
# Problem: Multiply
[code-task title="Multiply" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

[slide]
# Solution: Multiply
[code-task title="Multiply" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = Integer.parseInt(scanner.nextLine());
        for (int i = 1; i <= 10; i++) {
            int result = n * i;
            System.out.printf("%d x %d = %d%n",n, i, result);
        }
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