[slide]
# For Loop
Allows code to be executed **repeatedly**

Repeating while the condition is met

```java
for (initialization; condition; step {
       // Body of the for loop
}
```
**Initialization** - initializes the variable

**Condition** - evaluates the condition

**Step** - updates the initialized value

# For-Loop: Example

```java
for (int i = 1; i <= 10; i += 1) {
  System.out.println(i);
}
```
[/slide]

[slide]
# Problem: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads number **n** from the console
* Sums **all** numbers from **1** to **n**
* **Prints** the **sum** on the console

[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
15
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
55
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
28
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
3
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|

[/slide]

[slide]
# Solution: Print Sum of N Numbers
[code-task title="Print Sum of N Numbers" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = Integer.parseInt(scanner.nextLine());
        int sum = 0;
        for (int i = 1; i <= n; i += 1) {
            sum += i;
        }
        System.out.println(sum);
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads number **n** from the console
* Sums **all** numbers from **1** to **n**
* **Prints** the **sum** on the console

[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
15
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
55
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
28
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
3
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|5|15|
|6|21|

[/slide]

[slide]
# Problem: Calculate Month Salary
[code-task title="Calculate Month Salary" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads working **days** in the current month and **salary** per day
* **Calculates** the salary for the month
* Prints the result on the console

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
6
[/output]
[/test]
[test]
[input]
5
10
20
30
40
50
[/input]
[output]
150
[/output]
[/test]
[test]
[input]
3
10
234
54
[/input]
[output]
298
[/output]
[/test]
[test]
[input]
6
234
43
54
23
43
12
[/input]
[output]
409
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|3|60|
|10||
|20||
|30||

[/slide]

[slide]
# Solution: Calculate Month Salary
[code-task title="Calculate Month Salary" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int days = Integer.parseInt(scanner.nextLine());
        int totalSalary = 0;
        for (int i = 1; i <= days; i += 1) {
            int salaryPerDay = Integer.parseInt(scanner.nextLine());
            totalSalary += salaryPerDay;
        }
        System.out.println(totalSalary);
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads working **days** in the current month and **salary** per day
* **Calculates** the salary for the month
* Prints the result on the console


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
6
[/output]
[/test]
[test]
[input]
5
10
20
30
40
50
[/input]
[output]
150
[/output]
[/test]
[test]
[input]
3
10
234
54
[/input]
[output]
298
[/output]
[/test]
[test]
[input]
6
234
43
54
23
43
12
[/input]
[output]
409
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|3|60|
|10||
|20||
|30||

[/slide]