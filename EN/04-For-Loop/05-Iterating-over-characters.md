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
[code-task title="Latin Letters" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Latin Letters" executionStrategy="java-code" requiresInput]
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
[code-io /]
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