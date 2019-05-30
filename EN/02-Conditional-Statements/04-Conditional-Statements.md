[slide]
# Simple Conditions
Check certain **condition** and take action according to the result

```java
if (condition) {   //Boolean expression
  // Code for execution   
  // if the condition is true
}
```
The result is either **true** or **false**

[/slide]

[slide]
# Problem: Freezing Weather

[code-task title="Freezing Weather" executionStrategy="java-code" requiresInput]
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
* Reads a temperature in Celsius
* **Checks** whether the temperature is **below** zero
* Prints "**Freezing weather!**", if the temperature is equal or smaller than 0, otherwise print "**No output**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|4|(No output)|
|-2|Freezing weather!|


[/slide]

[slide]
# Solution: Freezing Weather

[code-task title="Freezing Weather" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double temperature = Double.parseDouble(scanner.nextLine());
        if (temperature <= 0) {
            System.out.println("Freezing weather!");
        }
        else {
            System.out.println("No output");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program, which:
* Reads a temperature in Celsius
* **Checks** whether the temperature is **below** zero
* Prints "**Freezing weather!**", if the temperature is equal or smaller than 0, otherwise print "**No output**"

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|4|(No output)|
|-2|Freezing weather!|

[/slide]