[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Guess the Password
[code-task title="Guess the Password" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads a string that is a **password**
* Prints "**Welcome**" if the password is "**s3cr3t**!"
* Prints "**Wrong password!**" in all other cases 

[/task-description]
[tests]
[test]
[input]
s3cr3t!
[/input]
[output]
Welcome
[/output]
[/test]
[test]
[input]
qwerty
[/input]
[output]
Wrong password!
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|

[/slide]

[slide]
# Solution: Guess the Password
[code-task title="Guess the Password" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String password = scanner.nextLine();
        if (password.equals("s3cr3t!")) {
          System.out.println("Welcome");
        } else {
          System.out.println("Wrong password!");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program which:
* Reads a string that is a **password**
* Prints "**Welcome**" if the password is "**s3cr3t**!"
* Prints "**Wrong password!**" in all other cases 

[/task-description]
[tests]
[test]
[input]
s3cr3t!
[/input]
[output]
Welcome
[/output]
[/test]
[test]
[input]
qwerty
[/input]
[output]
Wrong password!
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|s3cr3t!|Welcome|
|qwerty|Wrong password!|

[/slide]

[slide]
# Problem: Boiling Water
[code-task title="Boiling Water" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads a **floating-point** number
* Prints "**The water is boiling**" if the number > 100
* Prints "**The water is not hot enough**" in all other cases

[/task-description]
[tests]
[test]
[input]
104.8
[/input]
[output]
The water is boiling
[/output]
[/test]
[test]
[input]
29
[/input]
[output]
The water is not hot enough
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|

[/slide]

[slide]
# Solution: Boiling Water
[code-task title="Boiling Water" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]

```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double degrees = Double.parseDouble(scanner.nextLine());
      if (degrees > 100) {
        System.out.println("The water is boiling"); 
      } else {
        System.out.println("The water is not hot enough"); 
      }
    }
}
```
[/code-editor]
[task-description]

Write a program which:
* Reads a **floating-point** number
* Prints "**The water is boiling**" if the number > 100
* Prints "**The water is not hot enough**" in all other cases

[/task-description]
[tests]
[test]
[input]
104.8
[/input]
[output]
The water is boiling
[/output]
[/test]
[test]
[input]
29
[/input]
[output]
The water is not hot enough
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|104.8|The water is boiling|
|29|The water is not hot enough|

[/slide]

[slide]
# Problem: Speed Info
[code-task title="Speed Info" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads a floating-point number
* Prints "**Slow**" if the number **<=** 30
* Prints "**Fast**" if the number **>** 30

[/task-description]
[tests]
[test]
[input]
30
[/input]
[output]
Slow
[/output]
[/test]
[test]
[input]
60
[/input]
[output]
Fast
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|

[/slide]

[slide]
# Solution: Speed Info
[code-task title="Speed Info" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]

```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double speed = Double.parseDouble(scanner.nextLine());
      if (speed <= 30) {
        System.out.println("Slow");
      } else {
        System.out.println("Fast");
      }
    }
}
```
[/code-editor]
[task-description]

Write a program which:
* Reads a floating-point number
* Prints "**Slow**" if the number **<=** 30
* Prints "**Fast**" if the number **>** 30

[/task-description]
[tests]
[test]
[input]
30
[/input]
[output]
Slow
[/output]
[/test]
[test]
[input]
60
[/input]
[output]
Fast
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|30|Slow|
|60|Fast|

[/slide]

[slide]
# Problem: Area of Figures
[code-task title="Area of Figures" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads a type of figure
* Reads a **number** (**two numbers** for rectangle)
* Checks if the figure is **square**, **rectangle** or **circle**
* Prints the calculated area **formatted** to the **second decimal**
* For unknown figure print **"Unknown figure"**

[/task-description]
[tests]
[test]
[input]
square
5
[/input]
[output]
25.00
[/output]
[/test]
[test]
[input]
rectangle
5
10
[/input]
[output]
50.00
[/output]
[/test]
[test]
[input]
circle
2.5
[/input]
[output]
19.63
[/output]
[/test]
[test]
[input]
figure
[/input]
[output]
Unknown figure
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||

[/slide]

[slide]
# Solution: Area of Figures
[code-task title="Area of Figures" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]

```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String figure = scanner.nextLine();
        double area = 0;
        if (figure.equals("square")) {
            int side = Integer.parseInt(scanner.nextLine());
            area = side * side;
        } else if (figure.equals("rectangle")) {
            int width = Integer.parseInt(scanner.nextLine());
            int height = Integer.parseInt(scanner.nextLine());
            area = width * height;
        } else if (figure.equals("circle")) {
            double radius = Double.parseDouble(scanner.nextLine());
            area = Math.PI * (radius * radius);
        } else {
            System.out.println("Unknown figure");
            return;
        }
        System.out.printf("%.2f", area);
    }
}
```
[/code-editor]
[task-description]

Write a program which:
* Reads a type of figure
* Reads a **number** (**two numbers** for rectangle)
* Checks if the figure is **square**, **rectangle** or **circle**
* Prints the calculated area **formatted** to the **second decimal**

[/task-description]
[tests]
[test]
[input]
square
5
[/input]
[output]
25.00
[/output]
[/test]
[test]
[input]
rectangle
5
10
[/input]
[output]
50.00
[/output]
[/test]
[test]
[input]
circle
2.5
[/input]
[output]
19.63
[/output]
[/test]
[test]
[input]
figure
[/input]
[output]
Unknown figure
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|square|25.00|
|5||

[/slide]

[slide]
# Problem: Tickets
[code-task title="Tickets" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads a **ticket type** - either student or regular
* Prints the price in the following format "**$**{**price**}":
    * Student ticket is 1.00
    * Regular ticket is 1.60
    * For invalid type "Invalid ticket type!"

[/task-description]
[tests]
[test]
[input]
student
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
regular
[/input]
[output]
$1.60
[/output]
[/test]
[test]
[input]
ticket
[/input]
[output]
Invalid ticket type!
[/output]
[/test]
[/tests]
[/code-task]

|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|

[/slide]

[slide]
# Solution: Tickets
[code-task title="Tickets" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]

```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String ticketType = scanner.nextLine();
        if (ticketType.equals("student")) {
            System.out.println("$1.00");
        } else if (ticketType.equals("regular")) {
            System.out.println("$1.60");
        } else {
            System.out.println("Invalid ticket type!");
        }
    }
}
```
[/code-editor]
[task-description]

Write a program which:
* Reads a **ticket type** - either student or regular
* Prints the price in the following format "**$**{**price**}":
    * Student ticket is 1.00
    * Regular ticket is 1.60
    * For invalid type "Invalid ticket type!"

[/task-description]
[tests]
[test]
[input]
student
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
regular
[/input]
[output]
$1.60
[/output]
[/test]
[test]
[input]
ticket
[/input]
[output]
Invalid ticket type!
[/output]
[/test]
[/tests]
[/code-task]

|Input|Output|
|-----|------|
|student|$1.00|
|regular|$1.60|

[/slide]

[slide]
# Problem: Coffee Shop
[code-task title="Coffee Shop" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Reads an **order** - either "coffee" or "tea"
* Reads an **extra** - either "sugar" or "no"
* Prints a price in format "Final price: ${**price**}“
    * Price for coffee - 1.00
    * Price for tea - 0.60
    * Price for the sugar - 0.40

[/task-description]
[tests]
[test]
[input]
coffee
sugar
[/input]
[output]
Final price: $1.40
[/output]
[/test]
[test]
[input]
coffee
no
[/input]
[output]
Final price: $1.00
[/output]
[/test]
[test]
[input]
tea
sugar
[/input]
[output]
Final price: $1.00
[/output]
[/test]
[test]
[input]
tea
no
[/input]
[output]
Final price: $0.60
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|coffee|Final price: $1.40|
|sugar||

|Input|Output|
|-----|------|
|tea|Final price: $0.60|
|no||


[/slide]

[slide]
# Solution: Coffee Shop
[code-task title="Coffee Shop" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]

```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String order = scanner.nextLine();
        String extra = scanner.nextLine();
        double price = 0;
        if (order.equals("coffee")) {
            price = 1.00;
        } else if (order.equals("tea")) {
            price = 0.6;
        }
        if (extra.equals("sugar")) {
            price = price + 0.4;
        }
        System.out.printf("Final price: $%.2f", price);
    }
}
```

[/code-editor]
[task-description]

Write a program which:
* Reads an **order** - either "coffee" or "tea"
* Reads an **extra** - either "sugar" or "no"
* Prints a price in format "Final price: ${**price**}“
    * Price for coffee - 1.00
    * Price for tea - 0.60
    * Price for the sugar - 0.40

[/task-description]
[tests]
[test]
[input]
coffee
sugar
[/input]
[output]
Final price: $1.40
[/output]
[/test]
[test]
[input]
coffee
no
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
tea
sugar
[/input]
[output]
$1.00
[/output]
[/test]
[test]
[input]
tea
no
[/input]
[output]
$0.60
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|coffee|Final price: $1.40|
|sugar||

|Input|Output|
|-----|------|
|tea|Final price: $0.60|
|no||

[/slide]

[slide]
# Problem: Valid Triangle
[code-task title="Valid Triangle" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Write a program which:
* Receives **3 integers** - the **sides** of a **triangle**
* Checks if each **side** is **lesser** than the **sum** of the **other 2**
* Prints "Valid Triangle" if the above condition is met
* Prints "Invalid Triangle" otherwise

[/task-description]
[tests]
[test]
[input]
3
4
5
[/input]
[output]
Valid Triangle
[/output]
[/test]
[test]
[input]
5
8
3
[/input]
[output]
Invalid Triangle
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||

[/slide]

[slide]
# Solution: Valid Triangle
[code-task title="Valid Triangle" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int a = Integer.parseInt(scanner.nextLine());
        int b = Integer.parseInt(scanner.nextLine());
        int c = Integer.parseInt(scanner.nextLine());
        boolean isValidTriangle = true;
        if (a + b <= c) {
            isValidTriangle=false;
        } else if (a + c <= b) {
            isValidTriangle = false;
        } else if (b + c <= a) {
            isValidTriangle = false;
        }

        if (isValidTriangle) {
            System.out.println("Valid Triangle");
        }else {
            System.out.println("Invalid Triangle");
        }
    }
}
```

[/code-editor]
[task-description]

Write a program which:
* Receives **3 integers** - the **sides** of a **triangle**
* Checks if each **side** is **lesser** than the **sum** of the **other 2**
* Prints "Valid Triangle" if the above condition is met
* Prints "Invalid Triangle" otherwise

[/task-description]
[tests]
[test]
[input]
3
4
5
[/input]
[output]
Valid Triangle
[/output]
[/test]
[test]
[input]
5
8
3
[/input]
[output]
Invalid Triangle
[/output]
[/test]
[/tests]
[/code-task]

## Sample Input and Output
|Input|Output|
|-----|------|
|3|Valid Triangle|
|4||
|5||

[/slide]
