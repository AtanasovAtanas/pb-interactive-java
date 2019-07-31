[slide]
# For Loop with Step
The step part in a for loop can either increase or decrease the value of a variable
```java
for (int i = 0; i < 10; i += 2)
  System.out.println(i);
```
```java
for (int i = 10; i >= 0; i -= 2)
  System.out.println(i);
```
**Always pay attention to the condition**

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
* For each day prints: "**\{currentDay\} days before the exam**"
* At the end prints: "**The exam has come**"


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
* For each day prints: "**\{currentDay\} days before the exam**"
* At the end prints: "**The exam has come**"


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
[code-task title="Multiply" executionStrategy="java-code" requiresInput]
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
* Prints **n**'s first multiples in the format "**\{n\} x \{i\}** = **\{result\}**"

[/task-description]
[code-io /]
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
[code-task title="Multiply" executionStrategy="java-code" requiresInput]
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
* Prints **n**'s first multiples in the format "**\{n\} x \{i\}** = **\{result\}**"

[/task-description]
[code-io /]
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