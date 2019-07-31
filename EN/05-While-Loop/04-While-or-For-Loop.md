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
[code-task title="Odd Number" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
[tests]
[test]
[input]
5
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
4
6
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
2
7
[/input]
[output]
7
[/output]
[/test]
[test]
[input]
1
[/input]
[output]
1
[/output]
[/test]
[/tests]
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
[code-task title="Odd Number" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
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
[tests]
[test]
[input]
5
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
4
6
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
2
7
[/input]
[output]
7
[/output]
[/test]
[test]
[input]
1
[/input]
[output]
1
[/output]
[/test]
[/tests]
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
[code-task title="Number Processor" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
[tests]
[test]
[input]
5
Dec
Dec
End
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
8
Dec
Dec
Dec
Dec
End
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
3
Inc
End
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
1
Inc
Inc
Inc
[/input]
[output]
4
[/output]
[/test]
[/tests]
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
[code-task title="Number Processor" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
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
[tests]
[test]
[input]
5
Dec
Dec
End
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
8
Dec
Dec
Dec
Dec
End
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
3
Inc
End
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
1
Inc
Inc
Inc
[/input]
[output]
4
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5|6|
|Inc||
|End||
[/slide]
