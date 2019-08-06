[slide]
# Welcome to Programming
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

Check whether a specified subtext occurs within text
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

## Programming
**Programming** means writing computer programs (commands). 

Computer programs usually execute some algorithm. Algorithms are a sequence of steps, necessary for the completion of a certain task and for gaining some expected result, something like a "recipe". 

We need to use a certain **programming language**, such as C# or Python, to write it.

## Algorithms
**Algorithm** is a sequence of commands that achieves certain result. 

In programming the computer programs execute algorithms: a sequence of commands, necessary for the completion of a certain task. 

For example, to arrange a sequence of numbers in an ascending 
order, an algorithm is needed
  - e.g. find the smallest number and print it, then find the smallest number among the rest of the numbers and print it, and this is repeated until there are no more numbers left.

Programming is done by **programmers** (developers)

Programmers use IDE (like IntelliJ IDEA) to:

* **Write** the code
* **Run** and test the code
* Find a fix **bugs** (debug the code)
[/slide]

[slide]
# Computer Program – Example
Computer programs represent a sequence of commands that are written in certain programming language. 

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
The above program holds a sequence of 3 commands:
 * Declaring and assigning a variable: int size = 5;
 * Calculating and printing an expression: System.out.println("Size = " + size);
 * Calculating and printing an expression: System.out.println("Area = " + size * size);

 The result (output) from the above program is as follows:
```java
Size = 5
Area = 25
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

[slide]
# Video

[vimeo-video videoId="342593690" startTimeInSeconds="1783" endTimeInSeconds="3110" /]

[/slide]