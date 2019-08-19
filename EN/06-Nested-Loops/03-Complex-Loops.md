[slide]
# Complex Loops
Loops with different **steps**

The step is that part of the for loop construction that tells how much to **increase** or **decrease** the value of its leading variable. 

It is declared the last in the skeleton of the for loop.

Most often, we have a size of 1, and in this case, instead of writing i += 1 or i -= 1, we can use the **i++** or **i--** operators. 

If we want our step to be different than 1, when increasing, we use the i += + step size operator, and when decreasing, the i -= + step size.

```java
for (int i = n; i >= 1; i--) 
for (int j = 1; j <= n; j+=2)
for (int k = 1; k <= n; k*=2)
```
[/slide]

[slide]
# Problem: Numbers from N to 1
[code-task title="Numbers form N to 1" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[tests]
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
7
[/input]
[output]
7
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
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100|
||99|
||98|
||...|
||1|
[/slide]

[slide]
# Solution: Numbers from N to 1
[code-task title="Numbers form N to 1" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = Integer.parseInt(scanner.nextLine());
        
        for (int i = n; i >= 1; i--) {
            System.out.println(i);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **n** to **1** 
[/task-description]
[tests]
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
7
[/input]
[output]
7
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
# Sample Input and Output
|Input|Output|
|-----|------|
|100|100|
||99|
||98|
||...|
||1|
[/slide]

[slide]
# Problem: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
1
4
7
10
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
# Sample Input and Output
|Input|Output|
|-----|------|
|7|1|
||4|
||7|
[/slide]

[slide]
# Solution: Numbers from 1 to N with Step 3
[code-task title="Numbers from 1 to N with Step 3" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = Integer.parseInt(scanner.nextLine());
        for (int i = 1; i <= n; i += 3) {
            System.out.println(i);
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads an integer number **n**
* Prints the numbers from **1** to **n** with step **3**
[/task-description]
[tests]
[test]
[input]
4
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
5
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
10
[/input]
[output]
1
4
7
10
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
# Sample Input and Output
|Input|Output|
|-----|------|
|7|1|
||4|
||7|
[/slide]

[slide]
# Problem: Even Powers of 2
[code-task title="Even Powers of 2" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

* Reads a number **n**
* Prints the even powers of 2 to 2^**n**: 2^0, 2^2, 2^4, 2^8, …, 2^n
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
1
4
16
64
256
1024
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
1
4
16
64
256
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1|
||4|
||16|
||...|
||1024|
[/slide]

[slide]
# Solution: Even Powers of 2
[code-task title="Even Powers of 2" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        int n = Integer.parseInt(scanner.nextLine());
        int num = 1;
        for (int i = 0; i <= n; i += 2) {
            System.out.println(num);
            
            num = num * 2 * 2;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads a number **n**
* Prints the even powers of 2 to 2**n**: 20, 22, 24, 28, …, 2n
[/task-description]
[tests]
[test]
[input]
10
[/input]
[output]
1
4
16
64
256
1024
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
1
4
[/output]
[/test]
[test]
[input]
8
[/input]
[output]
1
4
16
64
256
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|10|1|
||4|
||16|
||...|
||1024|
[/slide]