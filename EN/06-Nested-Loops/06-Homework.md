[slide]
# Homework
Welcome to the homework. 

Now we are going to write a couple of console applications, by which we are going to make a few more steps into programming. 

We have prepared some problems for you to solve.

Let's solve a few problems to confirm what we have learned.

[image src="https://github.com/AtanasovAtanas/pb-interactive-csharp/blob/master/assets/homeowrk.png"/]
[/slide]

[slide]
# Problem: Building
[code-task title="Building" taskId="p-01" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Prints information about **apartments** (odd rows), **offices** (even rows) and the **last floor** (last row)
* Apartment `"A{buildingNum}{apartmentNum}"`
* Office `"O{floorNum}{officeNum}"`
* Floor `"L{buildingNum}{apartmentNum}"`
* The numbers always start from 0
# Example
## Input
- 6
- 4
## Output
- L60 L61 L62 L63
- A50 A51 A52 A53
- O40 O41 O42 O43
- A30 A31 A32 A33
- O20 O21 O22 O23
- A10 A11 A12 A13
[/task-description]
[tests]
[test]
[input]
1
7
[/input]
[output]
L10 L11 L12 L13 L14 L15 L16
[/output]
[/test]
[test]
[input]
0
0
[/input]
[output]

[/output]
[/test]
[test]
[input]
2
5
[/input]
[output]
L20 L21 L22 L23 L24
A10 A11 A12 A13 A14
[/output]
[/test]
[test]
[input]
10
10
[/input]
[output]
L100 L101 L102 L103 L104 L105 L106 L107 L108 L109
A90 A91 A92 A93 A94 A95 A96 A97 A98 A99
O80 O81 O82 O83 O84 O85 O86 O87 O88 O89
A70 A71 A72 A73 A74 A75 A76 A77 A78 A79
O60 O61 O62 O63 O64 O65 O66 O67 O68 O69
A50 A51 A52 A53 A54 A55 A56 A57 A58 A59
O40 O41 O42 O43 O44 O45 O46 O47 O48 O49
A30 A31 A32 A33 A34 A35 A36 A37 A38 A39
O20 O21 O22 O23 O24 O25 O26 O27 O28 O29
A10 A11 A12 A13 A14 A15 A16 A17 A18 A19
[/output]
[/test]
[test]
[input]
5
5
[/input]
[output]
L50 L51 L52 L53 L54
O40 O41 O42 O43 O44
A30 A31 A32 A33 A34
O20 O21 O22 O23 O24
A10 A11 A12 A13 A14
[/output]
[/test]
[test]
[input]
1
1
[/input]
[output]
L10
[/output]
[/test]
[test]
[input]
6
7
[/input]
[output]
L60 L61 L62 L63 L64 L65 L66
A50 A51 A52 A53 A54 A55 A56
O40 O41 O42 O43 O44 O45 O46
A30 A31 A32 A33 A34 A35 A36
O20 O21 O22 O23 O24 O25 O26
A10 A11 A12 A13 A14 A15 A16
[/output]
[/test]
[test]
[input]
8
2
[/input]
[output]
L80 L81
A70 A71
O60 O61
A50 A51
O40 O41
A30 A31
O20 O21
A10 A11
[/output]
[/test]
[test]
[input]
9
0
[/input]
[output]

[/output]
[/test]
[test]
[input]
7
3
[/input]
[output]
L70 L71 L72
O60 O61 O62
A50 A51 A52
O40 O41 O42
A30 A31 A32
O20 O21 O22
A10 A11 A12
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Passwords" taskId="p-02" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:
* Reads an integer - **n**
* Generates custom passwords, which meet the following conditions:
* The **first** part is an **even** number and should not be greater than **n**
* The **second** part is an **odd** number and should not be greater than **n**
* The **last part** is the **product** of the first two
# Example
## Input
- 6
## Output
- 212 236 2510 414 4312 4520 616 6318 6530
[/task-description]
[tests]
[test]
[input]
8
[/input]
[output]
212 236 2510 2714 414 4312 4520 4728 616 6318 6530 6742 818 8324 8540 8756
[/output]
[/test]
[test]
[input]
9
[/input]
[output]
212 236 2510 2714 2918 414 4312 4520 4728 4936 616 6318 6530 6742 6954 818 8324 8540 8756 8972
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
212 236 2510 2714 2918 414 4312 4520 4728 4936 616 6318 6530 6742 6954 818 8324 8540 8756 8972 10110 10330 10550 10770 10990
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
212 236
[/output]
[/test]
[test]
[input]
2
[/input]
[output]
212
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Magic Number" taskId="p-03" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:
* Reads a **number - n**, from the console
* Finds all **3-digit numbers** which product of the multiplication of their digits is equal to **n**
# Example
## Input
- 3
## Output
- 113
- 131
- 311
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
114
122
141
212
221
411
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Travelling" taskId="p-04" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads a **destination** and **needed budget** for destination
* Continues reading numbers - amounts of money, until they are **enough** for the destination
* If it receives the command **"End"** the program ends
# Example
## Input
- Philippines
- 1000
- 550
- 450
- End
## Output
- Going to Philippines!

[/task-description]
[tests]
[test]
[input]
Maldives
2500
1000
340
50
50
50
50
700
700
End
[/input]
[output]
Going to Maldives!
[/output]
[/test]
[test]
[input]
Bulgaria
500
200
100
300
Austria
700
200
200
200
200
End
[/input]
[output]
Going to Bulgaria!
Going to Austria!
[/output]
[/test]
[test]
[input]
Africa
3000
1000
5000
America
2000
2500
China
4000
2000
1800
1800
End
[/input]
[output]
Going to Africa!
Going to America!
Going to China!
[/output]
[/test]
[test]
[input]
Estonia
1000
300
200
200
300
Peru
3000
2000
1000
Uganda
1000
1000
UAE
5000
3000
4000
Germany
2000
2000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
Portugal
2050
3000
End
[/input]
[output]
Going to Estonia!
Going to Peru!
Going to Uganda!
Going to UAE!
Going to Germany!
Going to Portugal!
Going to Portugal!
Going to Portugal!
Going to Portugal!
Going to Portugal!
[/output]
[/test]
[test]
[input]
End
[/input]
[output]

[/output]
[/test]
[test]
[input]
France
3000
50
50
50
50
50
50
50
50
50
50
50
250
100
106
280
400
400
50
400
600
End
[/input]
[output]
Going to France!
[/output]
[/test]
[test]
[input]
Russia
15000
4500
300
300
3000
2000
4500
5000
Japan
1500.600
67.60
26.4052345
250.78
450.78945
578.76
98.60
260.84
End
[/input]
[output]
Going to Russia!
Going to Japan!
[/output]
[/test]
[test]
[input]
South Africa
2000
1000
1000
Egypt
300
150
100
20
20
20
End
[/input]
[output]
Going to South Africa!
Going to Egypt!
[/output]
[/test]
[test]
[input]
Zambia
3700.250
450.300
450.20414
600.43
640.23
824.50
1200.46
End
[/input]
[output]
Going to Zambia!
[/output]
[/test]
[test]
[input]
Albania
350.23414
45.24
23.124
123.144
145.23556
45.2345
End
[/input]
[output]
Going to Albania!
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Prime Numbers" taskId="p-05" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads **two numbers** from the console
* Prints the **prime** number in that **range**
# Example
## Input
- 1
- 50
## Output
- 1 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47
[/task-description]
[tests]
[test]
[input]
1
4
[/input]
[output]
1 2 3
[/output]
[/test]
[test]
[input]
600
900
[/input]
[output]
601 607 613 617 619 631 641 643 647 653 659 661 673 677 683 691 701 709 719 727 733 739 743 751 757 761 769 773 787 797 809 811 821 823 827 829 839 853 857 859 863 877 881 883 887
[/output]
[/test]
[test]
[input]
55
70
[/input]
[output]
59 61 67
[/output]
[/test]
[test]
[input]
11
13
[/input]
[output]
11 13
[/output]
[/test]
[test]
[input]
88
100
[/input]
[output]
89 97
[/output]
[/test]
[test]
[input]
23
27
[/input]
[output]
23
[/output]
[/test]
[test]
[input]
1
9
[/input]
[output]
1 2 3 5 7
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Unique PIN Codes" taskId="p-06" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads **3 digits** - n1, n2 and n3
* Generates **unique 3 digit PIN Codes**, which meet the following **conditions**:
* The **first** digit should not be greater than n1
* The **second** digit should not be greater than n2
* The **third** digit should not be greater than n3
* The **first** and the **third** digit must be even
* The second digit must be a **prime number** in the range \[2…7\]
# Example
## Input
- 3
- 5
- 5
## Output
- 222
- 224
- 232
- 234
- 252
- 254
[/task-description]
[tests]
[test]
[input]
8
2
8
[/input]
[output]
222
224
226
228
422
424
426
428
622
624
626
628
822
824
826
828
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Letter Combinations" taskId="p-07" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Prints **letters combinations** and the **count** of the printed combinations
* You will receive the **range of letters** on the first and second line
* On the third line, you will receive a **letter**, which you must **ignore** - don't print combinations with it
# Example
## Input
- a
- c
- b
## Output
- aaa aac aca acc caa cac cca ccc 8
[/task-description]
[tests]
[test]
[input]
a
c
b
[/input]
[output]
aaa aac aca acc caa cac cca ccc 8
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
[code-task title="Happy Numbers" taskId="p-08" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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
# Description
Write a program, which:

* Reads a number n
* Prints **all 4 digit numbers**, which meet the following conditions:
* When you **split** them in two pairs and **add** the first digit to the second - the result **equals** n
* When you add the first two digits to each other, the result must be **divisible** by n **without a remainder**
# Example
## Input
- 3
## Output
- 1212 1221 2112 2121
[/task-description]
[tests]
[test]
[input]
3
[/input]
[output]
1212 1221 2112 2121
[/output]
[/test]
[/tests]
[code-io/]
[/code-task]

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
