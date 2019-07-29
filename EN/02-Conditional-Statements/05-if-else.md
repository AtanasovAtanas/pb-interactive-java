[slide]
# If...else Statement
In an if-else statement, **`if`** condition evaluates to **`true`**, the then-statement runs. If condition is false, the else-statement runs

Because condition can't be simultaneously true and false, the then-statement and the else-statement of an if-else statement can never both run

In an if statement that doesn't include an else statement, if condition is true, the then-statement runs. If condition is false, control is transferred to the next statement after the if statement.

```java
if (condition) {
  // then-statement
  // Commands to be executed if the condition is true
} else {
  // else-statement
  // Commands to be executed if the condition is false
}
```
[/slide]

[slide]
# Block of Code
The curly brackets ***\{\}*** introduce a **block** (a group of commands)

In case the ***if*** statement does **not** have curly brackets, only the code on the **next line** will be executed

```java
String color = "red";
if (color.equals("red")) {
  System.out.println("tomato");
}else{
  System.out.println("banana");
}
System.out.println("lemon"); // Always executed
```

```java
String color = "red";
if (color.equals("red")) {    
    //block of 2 commands
  System.out.println("tomato");
  System.out.println("strawberry"); 
} else {
  //block of 3 commands
  System.out.println("banana");
  System.out.println("lemon");
  System.out.println("pear");
}

```

[/slide]

[slide]
# Problem: Even or Odd
[code-task title="Even or Odd" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Checks whether a number is **even** or **odd**
    * If it's even, it should print "**even**"
    * If it's odd, it should print "**odd**"

[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
91
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
105
[/input]
[output]
odd
[/output]
[/test]
[/tests]
[/code-task]



## Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|

[/slide]

[slide]
# Solution: Even or Odd

[code-task title="Even or Odd" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int num = Integer.parseInt(scanner.nextLine());
        if (num % 2 == 0) {
            System.out.println("even");
        } else {
            System.out.println("odd");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which: 
* Checks whether a number is **even** or **odd**
    * If it's even, it should print "**even**"
    * If it's odd, it should print "**odd**"

[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
even
[/output]
[/test]
[test]
[input]
91
[/input]
[output]
odd
[/output]
[/test]
[test]
[input]
105
[/input]
[output]
odd
[/output]
[/test]
[/tests]
[/code-task]



## Sample Input and Output
|Input|Output|
|-----|------|
|4|even|
|7|odd|

[/slide]

[slide]
# Problem: Greater Number
[code-task title="Greater Number" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads two **integers**
* Finds the greater number
* Prints "**Greater number:** " + the **greater** number

[/task-description]
[tests]
[test]
[input]
4
5
[/input]
[output]
Greater number: 5
[/output]
[/test]
[test]
[input]
100
1
[/input]
[output]
Greater number: 100
[/output]
[/test]
[test]
[input]
0
-1
[/input]
[output]
Greater number: 0
[/output]
[/test]
[test]
[input]
999
99
[/input]
[output]
Greater number: 999
[/output]
[/test]
[test]
[input]
-60
-70
[/input]
[output]
Greater number: -60
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|5|Greater number: 8|
|8|

[/slide]

[slide]
# Solution: Greater Number
[code-task title="Greater Number" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int num1 = Integer.parseInt(scanner.nextLine());
        int num2 = Integer.parseInt(scanner.nextLine());
        if (num1 > num2) {
            System.out.println("Greater number: " + num1);
        } else {
            System.out.println("Greater number: " + num2);
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads two **integers**
* Finds the greater number
* Prints "**Greater number:** " + the **greater** number

[/task-description]
[tests]
[test]
[input]
4
5
[/input]
[output]
Greater number: 5
[/output]
[/test]
[test]
[input]
100
1
[/input]
[output]
Greater number: 100
[/output]
[/test]
[test]
[input]
0
-1
[/input]
[output]
Greater number: 0
[/output]
[/test]
[test]
[input]
999
99
[/input]
[output]
Greater number: 999
[/output]
[/test]
[test]
[input]
-60
-70
[/input]
[output]
Greater number: -60
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|5|Greater number: 8|
|8|

[/slide]
