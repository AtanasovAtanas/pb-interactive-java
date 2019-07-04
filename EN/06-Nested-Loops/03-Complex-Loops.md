[slide]
# Complex Loops
Loops with different **steps**

```java
for (int i = n; i >= 1; i--) 
for (int j = 1; j <= n; j+=2)
for (int k = 1; k <= n; k*=2)
```
[/slide]

[slide]
# Problem: Numbers from N to 1
[code-task title="Numbers form N to 1" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Numbers form N to 1" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Numbers from 1 to N with Step 3" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Numbers from 1 to N with Step 3" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Even Powers of 2" executionStrategy="java-code" requiresInput]
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
[code-io /]
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
[code-task title="Even Powers of 2" executionStrategy="java-code" requiresInput]
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
[code-io /]
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