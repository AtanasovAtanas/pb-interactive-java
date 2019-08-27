[slide]
# Nested While Loops
```csharp
while (condition) {
  // Outer Loop 

  while (condition) {
    // Inner Loop
    
    // Statements
  }
}
```

# Nested While Loops - Example

```java
int i = 0;
while (i < 2) {
  System.out.printf($"Value of i: %d%n", i);
  
  int j = 1;
  i++;

  while (j < 2) {
    System.out.printf($"  Value of j: %d%n", j);
    j++;
  }
}

// Output
// Value of i: 0 
//  Value of j: 1 
//  Value of i: 1 
//  Value of j: 1 
```
[/slide]

[slide]
# Problem: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

* Reads the **height** of a triangle from the console
* Prints a **triangle of stars**
[/task-description]
[tests]
[test]
[input]
6
[/input]
[output]
*
**
***
****
*****
******
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
*
**
***
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
*
**
***
****
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]

[slide]
# Solution: Triangle of Stars with While
[code-task title="Triangle of Stars with While" executionType="tests-execution" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int height = Integer.parseInt(scanner.nextLine());
        int i = 1;

        while (i <= height) {
            int j = 1;
            while (j <= i) {
                System.out.print("*");
                j++;
            }

            System.out.println();
            i++;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

* Reads the **height** of a triangle from the console 
* Prints a **triangle of stars**
[/task-description]
[tests]
[test]
[input]
6
[/input]
[output]
*
**
***
****
*****
******
[/output]
[/test]
[test]
[input]
3
[/input]
[output]
*
**
***
[/output]
[/test]
[test]
[input]
4
[/input]
[output]
*
**
***
****
[/output]
[/test]
[/tests]
[/code-task]
# Sample Input and Output
|Input|Output|
|-----|------|
|5|*|
||**|
||***|
||****|
||*****|
[/slide]

[slide]
# Video

[vimeo-video videoId="345011935" startTimeInSeconds="4533" endTimeInSeconds="5149" /]

[/slide]