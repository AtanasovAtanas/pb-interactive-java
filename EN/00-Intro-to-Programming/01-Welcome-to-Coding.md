[slide]
# Welcome to programming
# What is Coding?
**Coding** means to give **commands** to tell the computer what to do

Sample command:
```java
System.out.println("I am coding");
```
A **computer program** is a sequence of commands
```java
System.out.println("First command");
System.out.println("Second command");
System.out.println("Third command");
```
[/slide]

[slide]
# Commands in Java – Examples 
Calculate an expression and print its value:
```java
System.out.println(5 + 5);
```
Plays the "A" sound (works in Windows only)
```java
System.out.println("softuni".contains("uni"));
```
Print the numbers from 1 to 100
```java
for (int i = 1; i <= 100; i++) 
    System.out.println(i);
```
[/slide]

[slide]
# Programming and Algorithms 
**Programming** means writing computer programs (commands)

* Using certain **programming language**, such as C# or Python

**Algorithm** == a sequence of commands that achieves certain result

Programming is done by **programmers** (developers)

Programmers use IDE (like IntelliJ IDEA) to:

* **Write** the code
* **Run** and test the code
* Find a fix **bugs** (debug the code)
[/slide]

[slide]
# Computer Program – Example
Sample Java program (sequence of Java commands):

```java
int size = 5;
System.out.println("Size = " + size);
System.out.println("Area = " + size * size);
```

[image src="https://github.com/AlenPaunov/pb-interactive-java/blob/master/assets/intro-to-programming-1.png"/]
[/slide]

[slide]
# Complete Computer Program
Sample complete Java program (class + method + commands):
```java
public class Main {
  public static void main(String[] args) {
    int size = 5;
    System.out.println("Size = " + size);
    System.out.println(
      "Area = " + size * size);
  }
}
```
[/slide]

[slide]
# Console-Based Java Program – Example
Java program, which converts from **USD** to **EUR**
```java
using System;

class Program
{
  public static void Main()
  {
    Scanner scanner = new Scanner(System.in);
    int dollars = scanner.nextInt();
    double euro = dollars * 0.883795087;
    System.out.print("Euro: " + euro);
  }
}
```
[/slide]
