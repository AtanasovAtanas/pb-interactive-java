[slide]
# Nested for Loops
Statements that consist of several **loops** located **inside each other**

**Nested loops** are used:

* To execute an **action**, which **executes** multiple **actions**
* To make more **complex** calculations and variations

```java
for (int i = 1; i <= n; i += 3)  {
   for (int j = 1; j <= n; j += 3) {
      for (int k = 1; k <= n; k += 3) {
        // Statements
      }
   }
}
```
[/slide]

[slide]
# Nested for Loops
The syntax for a **nested ***for*** loop in C#** is as follows

```csharp
for (init; condition; increment) {
  // Outer Loop 
  for (init; condition; increment) { 
    // Inner Loop

    // Statements
  }
}
```

```java
int a = 3;
int b = 3;
for (int i = 0; i < a; i++) {
    System.out.printf("i = %d%n", i);
    
    for (int j = 0; j < b; j++) {
        System.out.printf(" j = %d%n", j;
    }
}
```
[/slide]

[slide]
# Problem: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]

[slide]
# Solution: Triangle of Stars
[code-task title="Triangle of Stars" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int height = Integer.parseInt(scanner.nextLine());
        for (int i = 1; i <= height; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.println("*");
            }

            System.out.println();
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]