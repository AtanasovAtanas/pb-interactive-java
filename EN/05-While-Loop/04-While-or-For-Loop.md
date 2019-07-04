[slide]
# While or For Loop?
The while and for loops both repeat a block of code

Use for-loop when you preliminary know the number of iterations

* E.g. repeat exactly n times

Use while if you don't know when the exit condition will be met

* E.g. repeat until stopped
[/slide]

[slide]
# Problem: Odd Number
[code-task title="Odd Number" executionStrategy="java-code" requiresInput]
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

Write a program to enter an odd number

* Read numbers from the console until an odd number is entered

* Print the odd number as output
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
[/slide]

[slide]
# Solution: Odd Number
[code-task title="Odd Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      int num = scanner.nextInt();

      while (num % 2 == 0) {
        num = scanner.nextInt();
      }

      System.out.println(num);
    }
}
```
[/code-editor]
[task-description]

Write a program to enter an odd number

* Read numbers from the console until an odd number is entered

* Print the odd number as output
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|2|3|
|4||
|8||
|3||
[/slide]

[slide]
# Problem: Number Processor
[code-task title="Number Processor" executionStrategy="java-code" requiresInput]
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
Write a program to process a sequence of commands:

* Read an initial number from the input
* Read an execute a sequence of the following commands:

  * Inc – add 1 to the number (increment)
  * Dec – subtract 1 from the number (decrement)
  * End – print the number and stop the program
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Inc||
|End||
[/slide]

[slide]
# Solution: Number Processor
[code-task title="Number Processor" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      int number = Integer.parseInt(scanner.nextLine());
      String command = scanner.nextLine();

      while (!command.equals("End")) {
        switch (command) {
          case "Inc": 
            number++; 
            break;
          case "Dec": 
            number--; 
            break;
        }

        command = scanner.nextLine();
      }
      
      System.out.println(number);
    }
}
```
[/code-editor]
[task-description]
Write a program to process a sequence of commands:

* Read an initial number from the input
* Read an execute a sequence of the following commands:

  * Inc – add 1 to the number (increment)
  * Dec – subtract 1 from the number (decrement)
  * End – print the number and stop the program
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Inc||
|End||
[/slide]
