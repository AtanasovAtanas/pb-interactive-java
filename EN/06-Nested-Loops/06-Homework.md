[slide]
# Homework
Now, it's your turn to practice what you have learned in the training session.

We have prepared some simple problems for you to solve. If you struggle you can see the solution after each problem. 
[/slide]

[slide]
# Problem: Building
[code-task title="Building" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints information about **apartments** (odd rows), **offices** (even rows) and the **last floor** (last row)
* Apartment ***"A\{buildingNum\}\{apartmentNum\}"***
* Office ***"O\{floorNum\}\{officeNum\}"***
* Floor ***"L\{buildingNum\}\{apartmentNum\}"***
* The numbers always start from **0**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63|
|4|L60 A50 A51 A52 A53|
||O40 O41 O42 O43|
||A30 A31 A32 A33|
||O20 O21 O22 O23|
||A10 A11 A12 A13|
[/slide]

[slide]
# Solution: Building
[code-task title="Building" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int floors = Integer.parseInt(scanner.nextLine());
        int rooms = Integer.parseInt(scanner.nextLine());

        for (int currentFloor = floors; currentFloor >= 1; currentFloor--) {
            for (int currentRoom = 0; currentRoom < rooms; currentRoom++) {
                if (currentFloor == floors) {
                    System.out.printf("L%d%d ", currentFloor, currentRoom);
                } else if (currentFloor % 2 == 0) {
                    System.out.printf("O%d%d ", currentFloor, currentRoom);
                } else {
                    System.out.printf("A%d%d ", currentFloor, currentRoom);
                }
            }

            System.out.println();
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints information about **apartments** (odd rows), **offices** (even rows) and the **last floor** (last row)
* Apartment ***"A\{buildingNum\}\{apartmentNum\}"***
* Office ***"O\{floorNum\}\{officeNum\}"***
* Floor ***"L\{buildingNum\}\{apartmentNum\}"***
* The numbers always start from **0**
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|L60 L61 L62 L63|
|4|L60 A50 A51 A52 A53|
||O40 O41 O42 O43|
||A30 A31 A32 A33|
||O20 O21 O22 O23|
||A10 A11 A12 A13|
[/slide]

[slide]
# Problem: Passwords
[code-task title="Passwords" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Generates custom **3 digit** passwords, which meet the following conditions:
* The **first** digit is an **even** number
* The **second** digit is an **odd** number
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530|
|5|212 236 2510 414 4312 4520|
[/slide]

[slide]
# Solution: Passwords
[code-task title="Passwords" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = Integer.parseInt(scanner.nextLine());
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= n; j++) {
                if (i % 2 == 0 && j % 2 != 0) {
                    System.out.printf("%d%d%d ", i, j, i * j);
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Generates custom **3 digit** passwords, which meet the following conditions:
* The **first** digit is an **even** number
* The **second** digit is an **odd** number
* The **third** is the **product** of the first two
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|6|212 236 2510 414 4312 4520 616 6318 6530|
|5|212 236 2510 414 4312 4520|
[/slide]

[slide]
# Problem: Magic Number
[code-task title="Magic Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **number - n**, from the console
* Finds all **3-digit numbers**:
* Forming **n** as a product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113|
||131|
||311|
||111|
[/slide]

[slide]
# Solution: Magic Number
[code-task title="Magic Number" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int magicNumber = Integer.parseInt(scanner.nextLine());
        for (int i = 1; i <= 9; i++) {
            for (int j = 1; j <= 9; j++) {
                for (int k = 1; k <= 9; k++) {
                    if (i * j * k == magicNumber) {
                        System.out.printf("%d%d%d%n", i, j, k);
                    }
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **number - n**, from the console
* Finds all **3-digit numbers**:
* Forming **n** as a product of the multiplication of their digits
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|113|
||131|
||311|
||111|
[/slide]

[slide]
# Problem: Travelling
[code-task title="Travelling" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **destination** and **needed budget** for destination
* Continues reading numbers - amounts of money, until they are **enough** for the destination
* If it receives the command **"End"** the program ends
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Philippines|Going to Philippines!|
|1000||
|550||
|450||
|End||
[/slide]

[slide]
# Solution: Travelling
[code-task title="Travelling" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String townName = "";
        double currentMoney = 0;
        while (!(townName = scanner.nextLine()).equals("End")) {
            double neededMoney = Double.parseDouble(scanner.nextLine());

            while (currentMoney < neededMoney) {
                double money = Double.parseDouble(scanner.nextLine());
                currentMoney += money;
            }

            System.out.printf("Going to %s!%n", townName);
            currentMoney = 0;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a **destination** and **needed budget** for destination
* Continues reading numbers - amounts of money, until they are **enough** for the destination
* If it receives the command **"End"** the program ends
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|Philippines|Going to Philippines!|
|1000||
|550||
|450||
|End||
[/slide]

[slide]
# Problem: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads two numbers from the console
* Prints the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
[/slide]

[slide]
# Solution: Prime Numbers
[code-task title="Prime Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = Integer.parseInt(scanner.nextLine());
        int m = Integer.parseInt(scanner.nextLine());
        for (int num = n; num <= m; num++) {
            boolean prime = true;
            int divider = 2;
            int maxDivider = (int) Math.sqrt(num);

            while (divider <= maxDivider) {
                if (num % divider == 0) {
                    prime = false;
                    break;
                }

                divider++;
            }

            if (prime) {
                System.out.printf("%d ", num);
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads two numbers from the console
* Prints the prime number in that range
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|1|1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47|
|50||
[/slide]

[slide]
# Problem: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads 3 digits - each of them is an upper limit
* Generates unique 3 digit PIN Codes, which meet the following conditions:
* They are in the range
* The first and the third digit must be even
* The second digit must be a prime  number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Solution: Unique PIN Codes
[code-task title="Unique PIN Codes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n1 = Integer.parseInt(scanner.nextLine());
        int n2 = Integer.parseInt(scanner.nextLine());
        int n3 = Integer.parseInt(scanner.nextLine());

        for (int i = 1; i <= n1; i++) {
            for (int j = 1; j <= n2; j++) {
                for (int k = 1; k <= n3; k++) {
                    if (i % 2 == 0 && k % 2 == 0) {
                        if (j == 2 || j == 3 || j == 5 || j == 7) {
                            System.out.printf("%d%d%d%n", i, j, k);
                        }
                    }
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads 3 digits - each of them is an upper limit
* Generates unique 3 digit PIN Codes, which meet the following conditions:
* They are in the range
* The first and the third digit must be even
* The second digit must be a prime  number in the range \[2…7\]
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|222|
|5|224|
|5|232|
||234|
||252|
||254|
[/slide]

[slide]
# Problem: Letter Combinations
[code-task title="Letter Combinations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa aac aca acc caa cac cca ccc 8|
|c||
|b||
[/slide]

[slide]
# Solution: Letter Combinations
[code-task title="Letter Combinations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        char startLetter = scanner.nextLine().charAt(0);
        char endLetter = scanner.nextLine().charAt(0);
        char avoidLetter = scanner.nextLine().charAt(0);
        int counter = 0;

        for (char first = startLetter; first <= endLetter; first++) {
            for (char second = startLetter; second <= endLetter; second++) {
                for (char third = startLetter; third <= endLetter; third++) {
                    if (first != avoidLetter && second != avoidLetter && third != avoidLetter) {
                        System.out.printf("%c%c%c ", first, second, third);
                        counter++;
                    }
                }
            }
        }

        System.out.println(counter);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Prints letters combinations and the count of the printed combinations
* You will receive the range of letters on the first and second line
* On the third line, you will receive a letter, which you must ignore - don't print combinations with it
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|a|aaa aac aca acc caa cac cca ccc 8|
|c||
|b||
[/slide]

[slide]
# Problem: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number n
* Prints all 4 digit numbers, which meet the following conditions:
* When you split them in two pairs and add the first digit to the second - the result equals n
* When you add the first two digits to each other, the result must be divisible by n without a remainder
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1212 1221 2112 2121|
[/slide]

[slide]
# Solution: Happy Numbers
[code-task title="Happy Numbers" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int number = Integer.parseInt(scanner.nextLine());
        for (int firstDigit = 1; firstDigit <= 9; firstDigit++) {
            for (int secDigit = 1; secDigit <= 9; secDigit++) {
                for (int thirdDigit = 1; thirdDigit <= 9; thirdDigit++) {
                    for (int forthDigit = 1; forthDigit <= 9; forthDigit++) {
                        if (firstDigit + secDigit == thirdDigit + forthDigit &&
                                number % (firstDigit + secDigit) == 0) {
                            System.out.printf("%d%d%d%d ", firstDigit, secDigit, thirdDigit, forthDigit);
                        }
                    }
                }
            }
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number n
* Prints all 4 digit numbers, which meet the following conditions:
* When you split them in two pairs and add the first digit to the second - the result equals n
* When you add the first two digits to each other, the result must be divisible by n without a remainder
[/task-description]
[code-io /]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|3|1212 1221 2112 2121|
[/slide]
