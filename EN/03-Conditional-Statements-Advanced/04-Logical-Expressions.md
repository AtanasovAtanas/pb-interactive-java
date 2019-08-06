[slide]
# Logical Operators
Logical Operators are used to perform the logical operation between two operands like **AND**, **OR** and **NOT** based on our requirements

The Logical Operators will **always work with Boolean expressions** (**true** or **false**) and return **Boolean values**

The logical operators are:
  * AND (**&&**) - **returns true if both operands are true**
  * OR (**\| \|**) - **returns true if any one operand is true**
  * Logical negation (**!**) - **returns the reverse of logical state**
    * Brackets **()** change the order

| Operand1 | Operand2 | And | Or |
|---|---|---|---|
| true | true | true | true |
| true | false | false | true |
| false | true | false | true |
| false | false | false | false |

If you observe above table, **if any one operand value become false, then the logical AND operator will return false**, same way **the logical OR operator will return true, if any one operand value become true**

| Operand | Not |
|---|---|
| true | false |
| false | true |

If you observe above table, **the NOT operator will always return the reverse value of operand** like **if operand value true, then the Logical NOT operator will return false and vice versa**
[/slide]

[slide]
# Problem: Bonus Points
[code-task title="Bonus Points" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to add bonus to given points

* If points are between 0 and 3, adds 5
* If points are between 4 and 6, adds 15
* If points are between 7 and 9, adds 20
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
10
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
20
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
7
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
28
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Solution: Bonus Points
[code-task title="Bonus Points" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int points = Integer.parseInt(scanner.nextLine());
        if (points >= 0 && points <= 3) {
            points += 5;
        } else if (points >= 4 && points <= 6) {
            points += 15;
        } else if (points >= 7 && points <= 9) {
            points += 20;
        }
        
        System.out.println(points);
    }
}
```
[/code-editor]
[task-description]
Write a program to add bonus to given points

* If points are between 0 and 3, adds 5
* If points are between 4 and 6, adds 15
* If points are between 7 and 9, adds 20
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
10
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
20
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
7
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
28
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|4|19|
[/slide]

[slide]
# Problem: Food or Drink
[code-task title="Food or Drink" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
The result of the expression is ***true*** if one of the operands is ***true***, otherwise the result is ***false***

Check for food or drink

* Read single line and print "drink", "food" or "unknown"
* Foods: curry, noodles, sushi, spaghetti 
* Drinks: tea, water, coffee
* Everything else is unknown
[/task-description]
[tests]
[test]
[input]
curry
[/input]
[output]
food
[/output]
[/test]
[test]
[input]
tea
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
water
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
sushiiii
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Solution: Food or Drink
[code-task title="Food or Drink" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine();

        if (input.equals("curry") || input.equals("noodles") ||
                input.equals("sushi") || input.equals("spaghetti")) {
            System.out.println("food");
        } else if (input.equals("tea") || input.equals("water") ||
                input.equals("coffee")) {
            System.out.println("drink");
        } else {
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
[tests]
[test]
[input]
curry
[/input]
[output]
food
[/output]
[/test]
[test]
[input]
tea
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
water
[/input]
[output]
drink
[/output]
[/test]
[test]
[input]
sushiiii
[/input]
[output]
unknown
[/output]
[/test]
[/tests]
[/code-task]
[/slide]

[slide]
# Video

[vimeo-video videoId="341582556" startTimeInSeconds="2834" endTimeInSeconds="4109" /]

[/slide]