[slide]
# Problem: Greeting
[code-task title="Greeting" executionStrategy="java-code" requiresInput]
[code-editor language="java"]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      // Write code here
  }
}
```
[/code-editor]
[task-description]
Write a **program**, which:

* Reads a user input - **name**, from the console
* Prints "Hello, \{name\}!", where \{name\} is the user input
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Greeting
[code-task title="Greeting" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    String name = scanner.nextLine();
    System.out.print("Hello, ");
    System.out.println(name);
  }
}
```
[/code-editor]
[task-description]
Write a **program**, which:

* Reads a user input - **name**, from the console
* Prints "Hello, \{name\}!", where \{name\} is the user input
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Concatenating Text and Numbers
```java
String firstName = "John";
String lastName = "Doe";
int age = 34;
String str = firstName + " " + lastName + " | " + age;
System.out.println(str); // John Doe | 34

```

```java
int a = 5;
int b = 11;
String str = "a + b = " + a + b;
System.out.println(str); // a + b = 511
```
[/slide]

[slide]
# Arithmetic Operators
Adding numbers (operator **+** )
```java
int a = 5;
int b = 7;
int sum = a + b;
System.out.println(sum); // 12
```
Subtracting numbers (operator **-** )
```java
int a = 15;
int b = 7;
System.out.println(a - b); // 8
```
Multiplying numbers (operator **\***)
```java
int a = 5;
int b = 7;
System.out.println(a * b); // 35
```
Dividing numbers (operator **\/** )
```java
int a = 25;
int b = 4;
System.out.println(a / b); // 6
```
Modulo / remainder from integer division (operator **%**)
```java
int a = 7;
int b = 2;
System.out.println(a % b);   // 1
```
```java
System.out.println(3 % 2);   // 1
System.out.println(4 % 2);   // 0
System.out.println(3.5 % 1); // 0.5
```
[/slide]