[slide]
# Iterating over Characters
In Java, we can iterate over characters
```java
for (char ch = 'a'; ch <= 'd'; ch++) {
  System.out.println(ch + " ");
}
// Expected Output: a b c d
```
[/slide]

[slide]
# ASCII Table
Computers can only understand numbers
* **ASCII** code is the numerical representation of a character

|Dec|Hx|Oct|Html|Chr|
|---|--|---|----|---|
|97|61|141|\&\#97;|a|
|98|62|Oct|&\#98;|b|

[/slide]

[slide]
# Problem: Latin Letters
[code-task title="Latin Letters" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
* Reads **2 chars** from the console
* Prints **all letters** in the given range **inclusive**

[/task-description]
[tests]
[test]
[input]
a
m
[/input]
[output]
a b c d e f g h i j k l m
[/output]
[/test]
[test]
[input]
t
z
[/input]
[output]
t u v w x y z 
[/output]
[/test]
[test]
[input]
m
n
[/input]
[output]
m n
[/output]
[/test]
[test]
[input]
a
v
[/input]
[output]
a b c d e f g h i j k l m n o p q r s t u v 
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||

|Input|Output|
|-----|------|
|f|f g h i g k l|
|j||
[/slide]

[slide]
# Solution: Latin Letters
[code-task title="Latin Letters" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        char firstLetter = scanner.nextLine().charAt(0);
        char secondLetter = scanner.nextLine().charAt(0);

        for (char i = firstLetter; i <= secondLetter; i++) {
            System.out.print(i + " ");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads **2 chars** from the console
* Prints **all letters** in the given range **inclusive**

[/task-description]
[tests]
[test]
[input]
a
m
[/input]
[output]
a b c d e f g h i j k l m
[/output]
[/test]
[test]
[input]
t
z
[/input]
[output]
t u v w x y z 
[/output]
[/test]
[test]
[input]
m
n
[/input]
[output]
m n
[/output]
[/test]
[test]
[input]
a
v
[/input]
[output]
a b c d e f g h i j k l m n o p q r s t u v 
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|a b c|
|c||

|Input|Output|
|-----|------|
|f|f g h i g k l|
|j||
[/slide]