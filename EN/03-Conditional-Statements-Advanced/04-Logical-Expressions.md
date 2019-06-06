[slide]
# Conditional Operators
Used to perform logical operations

The logical operators in Java are:

* AND (**&&**)
* OR (**||**)
* Logical negation (**!**)

Brackets **()** change the order
[/slide]

[slide]
# Explanation

[image src="https://github.com/AlenPaunov/pb-interactive-course/blob/03-conditional-statements-advanced/assets/03-conditional-statements-advanced-1.png"/]
[/slide]

[slide]
# Problem: Bonus Points
[code-task title="Bonus Points" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Returns the Boolean value ***true*** if all of the operands are ***true*** and ***false*** otherwise

```java
if (x >= x1 && x <= x2 && y >= y1 && y <= y2)
```

Write a program to add bonus to given points

* If points are between 0 and 3, adds 5
* If points are between 4 and 6, adds 15
* If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Solution: Bonus Points
[code-task title="Bonus Points" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int points = Integer.parseInt(scanner.nextLine());
        if (points >= 0 && points <= 3)
            points += 5;
        else if (points >= 4 && points <= 6)
            points += 15;
        else if (points >= 7 && points <= 9)
            points += 20;
        System.out.println(points);
    }
}
```
[/code-editor]
[task-description]
Returns the Boolean value ***true*** if all of the operands are ***true*** and ***false*** otherwise

```java
if (x >= x1 && x <= x2 && y >= y1 && y <= y2)
```

Write a program to add bonus to given points

* If points are between 0 and 3, adds 5
* If points are between 4 and 6, adds 15
* If points are between 7 and 9, adds 20
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Problem: Food or Drink
[code-task title="Food or Drink" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
The result of the expression is ***true*** if one of the operands is ***true***, otherwise the result is ***false***

Check for food or drink

* Read single line and print "drink", "food" or "unknown"
* Foods: curry, noodles, sushi, spaghetti 
* Drinks: tea, water, coffee
* Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Food or Drink
[code-task title="Food or Drink" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
  public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String s = scanner.nextLine();
        if (s.equals("curry") || s.equals("noodles") || s.equals("sushi") || s.equals("spaghetti")) {
            System.out.println("food");
        }
        else if (s.equals("tea") || s.equals("water") || s.equals("coffee")) {
            System.out.println("drink");
        }
        else {
            System.out.println("unknown");
        }
    }
}
```
[/code-editor]
[task-description]
The result of the expression is ***true*** if one of the operands is ***true***, otherwise the result is ***false***

Check for food or drink

* Read single line and print "drink", "food" or "unknown"
* Foods: curry, noodles, sushi, spaghetti 
* Drinks: tea, water, coffee
* Everything else is unknown
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Logical NOT (!)
Logical negation returns ***true*** when the operand is ***false***, and ***false*** when the operand is ***true***

Example: check for valid number

* A number is valid if is in the range \[100…200\] or is equal to 0
[/slide]