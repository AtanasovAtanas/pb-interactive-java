[slide]
# While Loop
The **`while`** statement executes a statement or a block of statements while a specified **`Boolean expression`** evaluates to **`true`**

The expression is evaluated before each execution of the loop

```java
while (condition) {
   // commands
} 
```

# Example: Numbers from 1 to 5
```java
int i = 1;
while (i <= 5) {
   System.out.println(i);
   i++;
}
```
[/slide]

[slide]
# Problem: Decreasing Numbers
[code-task title="Decreasing Numbers" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Print the numbers from N down to 1, using a while loop

* Write a program which receives number: n

* Print the numbers n … 1
[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
3
2
1
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
4
3
2
1
[/output]
[/test]
[test]
[input]
6
[/input]
[output]
6
5
4
3
2
1
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Solution: Decreasing Numbers
[code-task title="Decreasing Numbers" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      int number = scanner.nextInt();
      while (number >= 1) {
         System.out.println(number);
         number--;
      }
    }
}
```
[/code-editor]
[task-description]
Print the numbers from N down to 1, using a while loop

* Write a program which receives number: n

* Print the numbers n … 1
[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
5
4
3
2
1
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
3
2
1
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
4
3
2
1
[/output]
[/test]
[test]
[input]
6
[/input]
[output]
6
5
4
3
2
1
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|4|4|
||3|
||2|
||1|
[/slide]

[slide]
# Problem: Number in Range
[code-task title="Number in Range" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to read a number in the range \[1 … 100\]:

* Read a number from the console
* Check if the number is in the range \[1 … 100\]

   * No -> read a new number
   * Yes -> print the number and the program stops
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
555
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
400
600
-1
6
[/input]
[output]
6
[/output]
[/test]
[test]
[input]
6
[/input]
[output]
6
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
[/slide]

[slide]
# Solution: Number in Range
[code-task title="Number in Range" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      int num = scanner.nextInt();
      while (num < 1 || num > 100) {
         num = scanner.nextInt();
      }
      System.out.println(num);
    }
}
```
[/code-editor]
[task-description]
Write a program to read a number in the range \[1 … 100\]:

* Read a number from the console
* Check if the number is in the range \[1 … 100\]

   * No -> read a new number
   * Yes -> print the number and the program stops
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
555
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
400
600
-1
6
[/input]
[output]
6
[/output]
[/test]
[test]
[input]
6
[/input]
[output]
6
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|-10|50|
|101||
|50||
[/slide]
