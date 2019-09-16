[slide]
# Problem: 3 Equal Numbers
[code-task title="Equal Numbers" executionType="tests-execution" executionStrategy="java-code" requiresInput]
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

Read **3** numbers from the console and print if they are **equal** (**yes/no**).

# Example

| **Input** | | **Output** |
| --- | --- | --- | 
| 1 | | yes | 
| 1 | | |
| 1 | | |

| **Input** | | **Output** |
| --- | --- | --- |
| 1| | no|
| 8| | |
| 5| | |
[/task-description]
[tests]
[test]
[input]
5
6
7
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
5
5
5
[/input]
[output]
yes
[/output]
[/test]
[test]
[input]
5
5
4
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
4
5
5
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
5
4
4
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
3
3
3
[/input]
[output]
yes
[/output]
[/test]
[test]
[input]
10
10
10
[/input]
[output]
yes
[/output]
[/test]
[test]
[input]
-1
-1
-1
[/input]
[output]
yes
[/output]
[/test]
[test]
[input]
7
8
9
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
1
1
2
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
1
2
1
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
2
1
1
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
12345
12346
12345
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
1
1
-1
[/input]
[output]
no
[/output]
[/test]
[test]
[input]
22222
22222
22223
[/input]
[output]
no
[/output]
[/test]
[/tests]
[code-io /]
[/code-task]
[/slide]