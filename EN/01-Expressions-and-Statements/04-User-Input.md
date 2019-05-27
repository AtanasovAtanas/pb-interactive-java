[slide]
# What is the Console (Terminal)?
The system **console** / **terminal** / **standard input and output**
* A special window, used to communicate with the user
* Using a **text-based** input / output (command line interface)
* Displays **text** data (text lines)
* Reads user **input** (text lines)

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/01-expressions-and-statements/assets/expressions-and-statements-1.png"/]

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/01-java-expressions-and-statements/assets/expressions-and-statements-2.png"/]

[/slide]

[slide]
# Reading User Input
Everything we receive from the console comes as a ***String***

Reading user input:
```java
Scanner scanner = new Scanner(System.in);
String name = scanner.nextLine();
```
Everything we print on the console is converted to ***String***
```java
System.out.println("Hello world!");
System.out.println("Hello" + 123);
```
[/slide]

[slide]
# Formatting Output
Formatting text with **placeholders**
```java
String firstName = "John";
int age = 19;
System.out.printf("%s is %d years old", firstName, age); //%s  - placeholder for text, %d  - placeholder for integer
// John is 19 years old
```

```java
double a = 5.123;
double b = 6.456;
System.out.printf("%.2f", a + b); //%f  - placeholder for floating-point number, %.2f - 2 digits after the decimal point
//11.58
```
[/slide]

[slide]
# Reading User Input
A program which **read**s a name from the console and **prints** it:
```java
Scanner scanner = new Scanner(System.in);
String name = scanner.nextLine();
System.out.println(name);
```
The result from the execution would be:
[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/01-java-expressions-and-statements/assets/expressions-and-statements-2.png"/]
[/slide]

[slide]
# Reading Integers
Reading an integer number:
```java
int num = Integer.parseInt(scanner.nextLine());
```
Example: 

* Calculating square's area by given side ***a***
```java
int a = Integer.parseInt(scanner.nextLine());
int area = a * a;
System.out.println(area);
```
[/slide]

[slide]
# Reading Floating-Point Numbers
Reading a floating-point number:
```java
double num = Double.parseDouble(scanner.nextLine());
```
Example: 

* Convert **inches** to **centimeters**
```java
double inches = Double.parseDouble(scanner.nextLine());
double centimeters = inches * 2.54;
System.out.println(centimeters);
```
[/slide]

[slide]
# Problem: Greeting
[code-task title="Greeting" executionStrategy="java-code" requiresInput]
[code-editor language="java"]
```java
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
```java
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
# Video

[youtube-video videoId="u811BV_KtkA" startTimeInSeconds="2902" endTimeInSeconds="6280" /]

[/slide]