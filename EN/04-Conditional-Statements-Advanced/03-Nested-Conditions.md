[slide]
# Nested Conditions
An ***if-else*** statement can be nested within another ***if-else*** statement

```java
if (expression) {
  if (nested expression)
    // Some code
  else
    // Some code
}
``` 

Only if the first condition is true the nested one is checked

```java
if (expression) {
  if (nested expression)
    // Some code
  else
    // Some code
    // Executes when the nested expression is false
}
```
Deep nesting is not recommended

* Use up to 3 nested levels

[/slide]

[slide]
# Problem: Marketplace
[code-task title="Marketplace" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Read a product and day from the console

Print the price, formatted to 2nd digit, based on the price table:

|Product|Weekday|Weekend|
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Kiwi|2.20|3.00|
[/task-description]
[tests]
[test]
[input]
Banana
Weekday
[/input]
[output]
2.50
[/output]
[/test]
[test]
[input]
Apple
Weekend
[/input]
[output]
1.60
[/output]
[/test]
[test]
[input]
Kiwi
Weekend
[/input]
[output]
3.00
[/output]
[/test]
[test]
[input]
Apple
Weekday
[/input]
[output]
1.30
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Kiwi|2.20|
|Weekday||

|Input|Output|
|-----|------|
|Banana|2.70|
|Weekend||
[/slide]

[slide]
# Solution: Marketplace
[code-task title="Marketplace" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String product = scanner.nextLine();
        String dayOfWeek = scanner.nextLine();

        if (product.equals("Banana")) {
            if (dayOfWeek.equals("Weekday")) {
                System.out.println("2.50");
            } else {
                System.out.println("2.70");
            }
        } else if (product.equals("Apple")) {
            if (dayOfWeek.equals("Weekday")) {
                System.out.println("1.30");
            } else {
                System.out.println("1.60");
            }
        } else if (product.equals("Kiwi"))
            if (dayOfWeek.equals("Weekday")) {
                System.out.println("2.20");
            } else {
                System.out.println("3.00");
            }
    }
}
```
[/code-editor]
[task-description]
Read a product and day from the console

Print the price, formatted to 2nd digit, based on the price table:

|Product|Weekday|Weekend|
|-------|-------|-------|
|Banana|2.50|2.70|
|Apple|1.30|1.60|
|Banana|2.20|3.00|
[/task-description]
[tests]
[test]
[input]
Banana
Weekday
[/input]
[output]
2.50
[/output]
[/test]
[test]
[input]
Apple
Weekend
[/input]
[output]
1.60
[/output]
[/test]
[test]
[input]
Kiwi
Weekend
[/input]
[output]
3.00
[/output]
[/test]
[test]
[input]
Apple
Weekday
[/input]
[output]
1.30
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Kiwi|2.20|
|Weekday||

|Input|Output|
|-----|------|
|Banana|2.70|
|Weekend||
[/slide]

[slide]
# Problem: Biggest Number of Three
[code-task title="Biggest Number of Three" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Read 3 numbers from the console

Print the biggest number of them
[/task-description]
[tests]
[test]
[input]
1
2
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
3
2
1
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
-2
0
4
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
-10
-11
-12
[/input]
[output]
-10
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|2|
|2||
|3||

|Input|Output|
|-----|------|
|1|5|
|5||
|3||
[/slide]

[slide]
# Solution: Biggest Number of Three
[code-task title="Biggest Number of Three" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int first = Integer.parseInt(scanner.nextLine());
        int second = Integer.parseInt(scanner.nextLine());
        int third = Integer.parseInt(scanner.nextLine());
        if (first > second)
            if (first > third) {
                System.out.println(first);
            } else {
                System.out.println(third);
            }
        else if (second > third) {
            System.out.println(second);
        } else {
            System.out.println(third);
        }
    }
}
```
[/code-editor]
[task-description]
Read 3 numbers from the console

Print the biggest number of them
[/task-description]
[tests]
[test]
[input]
1
2
3
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
3
2
1
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
-2
0
4
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
-10
-11
-12
[/input]
[output]
-10
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|2|
|2||
|3||

|Input|Output|
|-----|------|
|1|5|
|5||
|3||
[/slide]