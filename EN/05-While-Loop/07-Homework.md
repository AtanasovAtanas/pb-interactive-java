[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Sum Digits
[code-task title="Sum Digits" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to sum the digits of given number

* Read an integer from the console
* Sum its digits and print the sum
[/task-description]
[tests]
[test]
[input]
111
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
100004
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
121
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
554
[/input]
[output]
14
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|5634|18|
|150|6|
|-532|10|
[/slide]

[slide]
# Problem: Favorite Book
[code-task title="Favorite Book" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to guess for a favorite book, which: 

* Reads a favorite book's name
* Reads book names until it reaches the favorite book
* Prints "Book found!" and stops afterwards
* Prints "Invalid book: " + book for all invalid books
[/task-description]
[tests]
[test]
[input]
asd
fgh
asd
[/input]
[output]
Invalid book: fgh
Book found!
[/output]
[/test]
[test]
[input]
book
book
[/input]
[output]
Book found!
[/output]
[/test]
[test]
[input]
qwerty
asd
love
qwerty
[/input]
[output]
Invalid book: asd
Invalid book: love
Book found!
[/output]
[/test]
[test]
[input]
ooo
oo
o
ooo
[/input]
[output]
Invalid book: oo
Invalid book: o
Book found!
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|Alice in Wonderland|Invalid book: Winnie the Pooh|
|Winnie the Pooh|Book Found!|
|Alice in Wonderland||
[/slide]

[slide]
# Problem: Find Min and Max
[code-task title="Find Min and Max" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to find the min and max numbers

* Read integers from the console until "END" is entered
* Print the biggest and the smallest integer
[/task-description]
[tests]
[test]
[input]
1
2
3
END
[/input]
[output]
Min number: 1
Max number: 3
[/output]
[/test]
[test]
[input]
-4
5
10
30
END
[/input]
[output]
Min number: -4
Max number: 30
[/output]
[/test]
[test]
[input]
121
222
0
END
[/input]
[output]
Min number: 0
Max number: 222
[/output]
[/test]
[test]
[input]
554
-89
-8
23
END
[/input]
[output]
Min number: -89
Max number: 554
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|10|Min number: 0|
|20|Max number: 304|
|304||
|0||
|50||
|END||
[/slide]

[slide]
# Problem: Special Number
[code-task title="Special Number" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to check if given number is special: 

* Special numbers are divisible by all of their digits without remainder
* Read an integer and check whether it is a special number
* Print "\{num\} is special" if the number is special
* Otherwise, print "\{num\} is not special"
[/task-description]
[tests]
[test]
[input]
5
[/input]
[output]
5 is special
[/output]
[/test]
[test]
[input]
12
[/input]
[output]
12 i special
[/output]
[/test]
[test]
[input]
123
[/input]
[output]
123 is not special
[/output]
[/test]
[test]
[input]
567
[/input]
[output]
567 is not special
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|204|204 is special|
[/slide]

[slide]
# Solution: Special Number
[code-task title="Special Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      
      int num = Integer.parseInt(scanner.nextLine());
      int numDigits = num;
      boolean isSpecial = true;

      while (numDigits > 0) {
        int digit = numDigits % 10;
        numDigits /= 10;
        
        if (digit != 0 && num % digit != 0) {
          isSpecial = false;
          break;
        }
      }

      if (isSpecial) {
        System.out.println(num + " is special");
      } else {
        System.out.println(num + " is not special");
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to check if given number is special: 

* Special numbers are divisible by all of their digits without remainder
* Read an integer and check whether it is a special number
* Print "\{num\} is special" if the number is special
* Otherwise, print "\{num\} is not special"
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|23|23 is not special|
|204|204 is special|
[/slide]

[slide]
# Problem: Special Bonus
[code-task title="Special Bonus" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to apply a 20% bonus for certain number: 

* Read an integer from the console: the "stop number"
* Keep reading integers until it finds the stop number
* When the stop number is found, increase the value of the previous number before it with 20% and print it
[/task-description]
[tests]
[test]
[input]
111
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
100004
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
121
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
554
[/input]
[output]
14
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Solution: Special Bonus
[code-task title="Special Bonus" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      int stopNum = scanner.nextInt();
      int previousNum = stopNum;
      while (true) {
        int num = scanner.nextInt();
        if (num == stopNum)
          break;
        previousNum = num;
      }
      System.out.println(previousNum * 1.2);
    }
}
```
[/code-editor]
[task-description]
Write a program to apply a 20% bonus for certain number: 

* Read an integer from the console: the "stop number"
* Keep reading integers until it finds the stop number
* When the stop number is found, increase the value of the previous number before it with 20% and print it
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|25|36|
|20||
|30||
|25||
[/slide]

[slide]
# Problem: Sequence 2k + 1
[code-task title="Sequence 2k + 1" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to print a sequence of numbers:

* The first number is 1
* Each next number is 2 times the previous number + 1
* Read an integer n from the console – the max number
* Print the elements of the sequence, which are ≤ n
[/task-description]
[tests]
[test]
[input]
111
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
100004
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
121
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
554
[/input]
[output]
14
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
[/slide]

[slide]
# Solution: Sequence 2k + 1
[code-task title="Sequence 2k + 1" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      int n = scanner.nextInt();
      int k = 1;
      while (k <= n) {
        System.out.println(k);
        k = k * 2 + 1;
      }
    }
}
```
[/code-editor]
[task-description]
Write a program to print a sequence of numbers:

* The first number is 1
* Each next number is 2 times the previous number + 1
* Read an integer n from the console – the max number
* Print the elements of the sequence, which are ≤ n
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|8|1|
||3|
||7|
[/slide]

[slide]
# Problem: Account Balance
[code-task title="Account Balance" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
Write a program to calculate an account balance 

* Read a sequence of incomes / expenses, until "End" is read
* Add the money to the balance (starting form 0) and print "Increase: \{money\} " or "Decrease: \{money\}"
* Finally, print the account balance
[/task-description]
[tests]
[test]
[input]
111
[/input]
[output]
3
[/output]
[/test]
[test]
[input]
100004
[/input]
[output]
5
[/output]
[/test]
[test]
[input]
121
[/input]
[output]
4
[/output]
[/test]
[test]
[input]
554
[/input]
[output]
14
[/output]
[/test]
[/tests]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|500|Increase: 500.00|
|15.5|Increase: 15.50|
|-80.35|Decrease: 80.35|
|End|Balance: 435.15|
[/slide]

[slide]
# Solution: Account Balance
[code-task title="Account Balance" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```java
import java.util.Scanner;

public class Program {
   public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      double balance = 0.0;
      while (true) {
        String input = scanner.nextLine();
        if (input.equals("End")) break;
        double amount = Double.parseDouble(input);
        balance += amount;
        if (amount >= 0)
          System.out.printf("Increase: %.2f\n", amount);
        else
          System.out.printf("Decrease: %.2f\n", -amount);
      }
      System.out.printf("Balance: %.2f\n", balance);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate an account balance 

* Read a sequence of incomes / expenses, until "End" is read
* Add the money to the balance (starting form 0) and print "Increase: \{money\} " or "Decrease: \{money\}"
* Finally, print the account balance
[/task-description]
[code-io /]
[/code-task]
## Sample Input and Output
|Input|Output|
|-----|------|
|500|Increase: 500.00|
|15.5|Increase: 15.50|
|-80.35|Decrease: 80.35|
|End|Balance: 435.15|
[/slide]
