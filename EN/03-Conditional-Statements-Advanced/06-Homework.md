[slide]
# Homework
Welcome to the homework. 

Now we are going to write a couple of console applications, by which we are going to make a few more steps into programming. 

We have prepared some problems for you to solve.

Let's solve a few problems to confirm what we have learned.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/homeowrk.png"/]
[/slide]

[slide]
# Problem: Fruit or Vegetable
[code-task title="Fruit or Vegetable" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: **"vegetable"**, **"fruit"** or **"unknown"**
# Example
## Input
- lemon
## Output
- fruit
## Input
- carrot
## Output
- vegetable
[/task-description]
[tests]
[test]
[input]
lemon
[/input]
[output]
fruit
[/output]
[/test]
[test]
[input]
carrot
[/input]
[output]
vegetable
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Fruit or Vegetable
[code-task title="Fruit or Vegetable" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Program {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String product = scanner.nextLine();
        switch (product) {
            case "cucumber":
            case "pepper":
            case "carrot":
                System.out.println("vegetable");
                break;
            case "banana":
            case "apple":
            case "kiwi":
            case "cherry":
            case "lemon":
            case "grapes":
                System.out.println("fruit");
                break;
            default:
                System.out.println("unknown");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to check for fruit or vegetable:

* Read a single input line: an item from the greengrocery
* Fruits: banana, apple, kiwi, cherry, lemon, grapes
* Vegetables: cucumber, pepper, carrot, onion
* Print: "vegetable", "fruit" or "unknown"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|lemon|fruit|
|carrot|vegetable|
[/slide]

[slide]
# Problem: Day of Week
[code-task title="Day of Week" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to print the day of week as words:

* Read and integer **n**: the **day of the week** in range [1..7]
* Print the **name of the day** (as words, in English)
* Print **"Error"** if the number is not in the given range
# Example
## Input
- 1
## Output
- Monday
## Input
- 8
## Output
- Error
[/task-description]
[tests]
[test]
[input]
1
[/input]
[output]
Monday
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
Error
[/output]
[/test]
[test]
[input]
7
[/input]
[output]
Sunday
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Day of Week
[code-task title="Day of Week" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int day = Integer.parseInt(scanner.nextLine());
        switch (day) {
            case 1:
                System.out.println("Monday");
                break;
            case 2:
                System.out.println("Tuesday");
                break;
            case 3:
                System.out.println("Wednesday");
                break;
            case 4:
                System.out.println("Thursday");
                break;
            case 5:
                System.out.println("Friday");
                break;
            case 6:
                System.out.println("Saturday");
                break;
            case 7:
                System.out.println("Sunday");
                break;
            default:
                System.out.println("Error");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to print the day of week as words:

* Read and integer n: the day of the week in range [1..7]
* Print the name of the day (as words, in English)
* Print "Error" if the number is not in the given range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Monday|
|8|Error|
|7|Sunday|
[/slide]

[slide]
# Problem: Vowel or Consonant
[code-task title="Vowel or Consonant" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to check a letter for vowel or consonant:

* Read a **letter** from the English alphabet
* Print either **"Vowel"** or **"Consonant"**
# Example
## Input
- a
## Output
- Vowel
## Input
- B
## Output
- Consonant
[/task-description]
[tests]
[test]
[input]
a
[/input]
[output]
Vowel
[/output]
[/test]
[test]
[input]
E
[/input]
[output]
Vowel
[/output]
[/test]
[test]
[input]
b
[/input]
[output]
Consonant
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Vowel or Consonant
[code-task title="Vowel or Consonant" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        char letter = scanner.nextLine().charAt(0);

        if (letter == 'A' || letter == 'a' ||
                letter == 'E' || letter == 'e' ||
                letter == 'I' || letter == 'i' ||
                letter == 'O' || letter == 'o' ||
                letter == 'U' || letter == 'u') {
            System.out.println("Vowel");
        } else {
            System.out.println("Consonant");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to check a letter for vowel or consonant:

* Read a letter from the English alphabet
* Print either "Vowel" or "Consonant"
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|Vowel|
|E|Vowel|
|b|Consonant|
[/slide]

[slide]
# Problem: Product of 3 Numbers
[code-task title="Product of 3 Numbers" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Calculate the sign of the product of 3 numbers:

* Read **3 floating-point** numbers
* Print the **sign** of the product of the entered 3 numbers: **positive**, **negative** or **zero**

Try to do this **without multiplying** the 3 numbers
# Example
## Input
- 2
- 3
- -1
## Output
- negative
[/task-description]
[tests]
[test]
[input]
-2
3
1
[/input]
[output]
negative
[/output]
[/test]
[test]
[input]
-3
-4
5
[/input]
[output]
positive
[/output]
[/test]
[test]
[input]
1
2
0
[/input]
[output]
zero
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Product of 3 Numbers
[code-task title="Product of 3 Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double n1 = Double.parseDouble(scanner.nextLine());
        double n2 = Double.parseDouble(scanner.nextLine());
        double n3 = Double.parseDouble(scanner.nextLine());

        if (n1 == 0 || n2 == 0 || n3 == 0) {
            System.out.println("zero");
        } else {
            int negativeNumbersCount = 0;
            if (n1 < 0) {
                negativeNumbersCount += 1;
            }

            if (n2 < 0) {
                negativeNumbersCount += 1;
            }

            if (n3 < 0) {
                negativeNumbersCount += 1;
            }

            if (negativeNumbersCount % 2 == 0) {
                System.out.println("positive");
            } else {
                System.out.println("negative");
            }
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the sign of the product of 3 numbers:

* Read 3 floating-point numbers
* Print the sign of the product of the entered 3 numbers: positive, negative or zero

Try to do this without multiplying the 3 numbers

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|2|negative|
|3||
|-1||
|-3|positive|
|-4||
|5||
[/slide]

[slide]
# Problem: Sorted Numbers
[code-task title="Sorted Numbers" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program, which checks for **sorted 3 numbers**:

* Read 3 real numbers
* Print **"Ascending"** if the numbers are in ascending order
* Print **"Descending"** if the numbers are in descending order
* Print **"Not sorted"** in any other case
# Example
## Input
- 1
- 2
- 3
## Output
- Ascending
## Input
- 3
- 5
- 2
## Output
- Not sorted
[/task-description]
[tests]
[test]
[input]
1
2
3
[/input]
[output]
Ascending
[/output]
[/test]
[test]
[input]
3
1
2
[/input]
[output]
Not sorted
[/output]
[/test]
[test]
[input]
3
2
1
[/input]
[output]
Descending
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Sorted Numbers
[code-task title="Sorted Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double n1 = Double.parseDouble(scanner.nextLine());
        double n2 = Double.parseDouble(scanner.nextLine());
        double n3 = Double.parseDouble(scanner.nextLine());

        if (n1 < n2 && n2 < n3) {
            System.out.println("Ascending");
        } else if (n1 > n2 && n2 > n3) {
            System.out.println("Descending");
        } else {
            System.out.println("Not sorted");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which checks for sorted 3 numbers:

* Read 3 real numbers
* Print "Ascending" if the numbers are in ascending order
* Print "Descending" if the numbers are in descending order
* Print "Not sorted" in any other case

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|Ascending|
|2||
|3||
|3|Not sorted|
|1||
|2||
[/slide]

[slide]
# Problem: Vacation Expenses
[code-task title="Vacation Expenses" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
# Description
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Example
## Input
- Winter
- Hotel
- 5
## Output
- 180.00
[/task-description]
[tests]
[test]
[input]
Winter
Hotel
5
[/input]
[output]
180.00
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Vacation Expenses
[code-task title="Vacation Expenses" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String season = scanner.nextLine();
        String accommodation = scanner.nextLine();
        int days = Integer.parseInt(scanner.nextLine());
        double totalPrice = 0.0;

        if (season.equals("Spring")) {
            if (accommodation.equals("Hotel")) {
                totalPrice = days * 30 * 0.80;
            } else if (accommodation.equals("Camping")) {
                totalPrice = days * 10 * 0.80;
            }
        } else if (season.equals("Summer")) {
            if (accommodation.equals("Hotel")) {
                totalPrice = days * 50;
            } else if (accommodation.equals("Camping")) {
                totalPrice = days * 30;
            }
        } else if (season.equals("Autumn")) {
            if (accommodation.equals("Hotel")) {
                totalPrice = days * 20 * 0.7;
            } else if (accommodation.equals("Camping")) {
                totalPrice = days * 15 * 0.7;
            }
        } else if (season.equals("Winter")) {
            if (accommodation.equals("Hotel")) {
                totalPrice = days * 40 * 0.9;
            } else if (accommodation.equals("Camping")) {
                totalPrice = days * 10 * 0.9;
            }
        }

        System.out.printf("%.2f", totalPrice);
    }
}
```
[/code-editor]
[task-description]
Write a program, which calculates vacation expenses:

* Read season, accommodation type and count of the days
* Print the total expenses, based on the price table bellow,formatted to the 2nd * digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Season|Hotel|Camping|Discount|
|-----|------|-------|--------|
|Spring|30|10|20%|
|Summer|50|30|0%|
|Autumn|20|15|30%|
|Winter|40|10|10%|
# Sample Input and Output
|Input|Output|
|-----|------|
|Winter|180.00|
|Hotel||
|5||
[/slide]

[slide]
# Problem: Cinema
[code-task title="Cinema" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Calculate the **price** for all the tickets for a cinema movie:

* Reads the **type of the movie**, the **rows** and the **seats per row** in the cinema
* Prints the **total price** for all seats **formatted** to the 2nd digit after the decimal point

|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|

# Example
## Input
- Normal
- 12
- 9
## Output
- 810.00
[/task-description]
[tests]
[test]
[input]
Normal
12
9
[/input]
[output]
810.00
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Cinema
[code-task title="Cinema" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String type = scanner.nextLine();
        int rows = Integer.parseInt(scanner.nextLine());
        int cols = Integer.parseInt(scanner.nextLine());
        int seats = rows * cols;

        switch (type) {
            case "Premiere":
                System.out.printf("%.2f", seats * 12.0);
                break;
            case "Normal":
                System.out.printf("%.2f", seats * 7.50);
                break;
            case "Discount":
                System.out.printf("%.2f", seats * 5.00);
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Calculate the price for all the tickets for a cinema movie:

* Reads the type of the movie, the rows and the seats per row in the cinema
* Prints the total price for all seats formatted to the 2nd digit after the decimal point

[/task-description]
[code-io /]
[/code-task]
|Type|Price|
|-----|----|
|Premiere|12.00|
|Normal|7.50|
|Discount|5.00|
# Sample Input and Output
|Input|Output|
|-----|------|
|Normal|810.00|
|12||
|9||
[/slide]

[slide]
# Problem: Operations with Numbers
[code-task title="Operations with Numbers" taskId="p-08" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to apply an operator for given two numbers:

* Read **two integers** and **math operator** from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following **format**: "\{N1\} \{operator\} \{N2\} = \{result\}"
# Example
## Input
- 12
- 10
- \+
## Output
- 12 + 10 = 22
[/task-description]
[tests]
[test]
[input]
10
12
+
[/input]
[output]
10 + 12 = 22
[/output]
[/test]
[test]
[input]
12
10
\-
[/input]
[output]
12 \- 10 = 2
[/output]
[/test]
[test]
[input]
10
12
*
[/input]
[output]
10 * 12 = 120
[/output]
[/test]
[test]
[input]
6
2
/
[/input]
[output]
6 / 2 = 3
[/output]
[/test]
[test]
[input]
5
2
%
[/input]
[output]
5 % 2 = 1
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Operations with Numbers
[code-task title="Operations with Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int num1 = Integer.parseInt(scanner.nextLine());
        int num2 = Integer.parseInt(scanner.nextLine());
        char operation = scanner.nextLine().charAt(0);

        int result = 0;
        if (operation == '+') {
            result = num1 + num2;
        } else if (operation == '-') {
            result = num1 - num2;
        } else if (operation == '*') {
            result = num1 * num2;
        } else if (operation == '/') {
            result = num1 / num2;
        } else if (operation == '%') {
            result = num1 % num2;
        }

        System.out.printf("%d %s %d = %d", num1, operation, num2, result);
    }
}
```
[/code-editor]
[task-description]
Write a program to apply an operator for given two numbers:

* Read two integers and math operator from the console
* The math operator could be: "+", "-", "/", "%" and "*"
* The output should be in the following format: "\{N1\} \{operator\} \{N2\} = \{result\}"

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|10 + 12 = 22|
|12||
|+||
[/slide]

[slide]
# Problem: ATM
[code-task title="ATM" taskId="p-09" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to simulate an ATM withdrawal:

* Read: **balance**, **withdraw** and **limit**
* Print **"The withdraw was successful."** if the balance is enough
* Print **"The daily limit was exceeded."** if the limit is exceeded
* Print **"Insufficient availability."** if the balance isn't enough

# Example
## Input
- 420
- 20
- 25
## Output
- The withdraw was successful.
## Input
- 10
- 50
- 20
## Output
- The daily limit was exceeded.
- Insufficient availability.
[/task-description]
[tests]
[test]
[input]
420
20
25
[/input]
[output]
The withdraw was successful.
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: ATM
[code-task title="ATM" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int balance = Integer.parseInt(scanner.nextLine());
        int withdraw = Integer.parseInt(scanner.nextLine());
        int limit = Integer.parseInt(scanner.nextLine());

        if (balance >= withdraw && withdraw <= limit) {
            System.out.println("The withdraw was successful.");
        } else if (withdraw > limit) {
            System.out.println("The daily limit was exceeded.");
        } else if (withdraw > balance) {
            System.out.println("Insufficient availability.");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to simulate an ATM withdrawal:

* Read: balance, withdraw and limit
* Print "The withdraw was successful." if the balance is enough
* Print "The daily limit was exceeded." if the limit is exceeded
* Print "Insufficient availability." if the balance isn't enough

[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|420|The withdraw was successful.|
|20||
|25||
|10|The daily limit was exceeded.|
|50|Insufficient availability.|
|20||
[/slide]

[slide]
# Problem: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" taskId="p-10" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    }
}
```
[/code-editor]
[task-description]
# Description
Write a program to find the biggest among 5 numbers
* Read **5 integers**
* Print the **biggest** number
# Example
## Input
- -1
- -2
- -3
- -4
- -5
## Output
- -1
[/task-description]
[tests]
[test]
[input]
1
2
3
4
5
[/input]
[output]
5
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

[/slide]

[slide]
# Solution: Biggest of Five Numbers
[code-task title="Biggest of Five Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int num1 = Integer.parseInt(scanner.nextLine());
        int num2 = Integer.parseInt(scanner.nextLine());
        int num3 = Integer.parseInt(scanner.nextLine());
        int num4 = Integer.parseInt(scanner.nextLine());
        int num5 = Integer.parseInt(scanner.nextLine());

        if (num1 >= num2 && num1 >= num3 && num1 >= num4 && num1 >= num5) {
            System.out.println(num1);
        } else if (num2 >= num1 && num2 >= num3 && num2 >= num4 && num2 >= num5) {
            System.out.println(num2);
        } else if (num3 >= num1 && num3 >= num2 && num3 >= num4 && num3 >= num5) {
            System.out.println(num3);
        } else if (num4 >= num1 && num4 >= num2 && num5 >= num3 && num4 >= num5) {
            System.out.println(num4);
        } else if (num5 >= num1 && num5 >= num2 && num5 >= num3 && num5 >= num4) {
            System.out.println(num5);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program to find the biggest among 5 numbers
* Read 5 integers
* Print the biggest number
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|5|
|2||
|3||
|4||
|5||
|-1|-1|
|-2||
|-3||
|-4||
|-5||
[/slide]