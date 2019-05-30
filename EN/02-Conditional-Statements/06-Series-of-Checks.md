[slide]
# Sequence of Conditions
Sometimes we need to do a sequence of conditions before we decide what actions our program will execute. In such cases, we can apply the construction if-else if ... -else in series. For this purpose, we use the following format:

```java
//If one condition is true, the program will NOT check the rest of the conditions
if (...) {
// Execution code
} else if (...) {
// Execution code
} else if (...) {
// Execution code
}
```
[/slide]

[slide]
# Series of Conditions - Example
The program checks the first condition, finds that it is true and ends

```java
int a = 7;
if (a > 4) 
  System.out.println("Bigger than 4"); 
else if (a > 5)
  System.out.println("Bigger than 5"); 
else 
  System.out.println("Equal to 7"); 

//The output is only "Bigger than 4" 
```

[/slide]

[slide]
# Problem: Number 1…9
[code-task title="Problem: Number 1…9" executionStrategy="java-code" requiresInput]
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
* Reads an **integer** and checks its value [1, 9]
* Prints the value in the form of text
* If the number is **greater** than 9 prints "**Number too big**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|

[/slide]

[slide]
# Solution: Number 1…9
[code-task title="Problem: Number 1…9" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int num =
                Integer.parseInt(scanner.nextLine());
        if (num == 1) {
            System.out.println("one");
        }
        // TODO: Add the rest of the conditions
        else {
            System.out.println("Number too big");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which: 
* Reads an **integer** and checks its value [1, 9]
* Prints the value in the form of text
* If the number is **greater** than 9 prints "**Number too big**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|7|seven|
|10|Number too big|

[/slide]