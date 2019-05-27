[slide]
# Arithmetic Operators

# Arithmetic Operators: + and -
Adding numbers (operator **+** )
```java
int a = 5;
int b = 7;
int sum = a + b;
System.out.println(sum); // 12
```
Subtracting numbers (operator **-** )
```java
int a = 15;
int b = 7;
System.out.println(a - b); // 8
```
[/slide]

[slide]
# Arithmetic Operators: * and /
Multiplying numbers (operator **\***)
```java
int a = 5;
int b = 7;
System.out.println(a * b); // 35
```
Dividing numbers (operator **\/** )
```java
int a = 25;
int b = 4;
System.out.println(a / b); // 6
```
[/slide]

[slide]
# Division Behavior in Java
When dividing integers, the result is also integer:
```java
int a = 25;
System.out.println(a / 4);  // Integer result: 6
System.out.println(a / 0);  // Error: division by 0
```
When dividing floating-points, the result is also floating-point:
```java
double a = 15;
System.out.println(a / 2.0); // 7.5
System.out.println(a / 0.0); // Infinity
System.out.println(0 / 0.0); // NaN
```
[/slide]

[slide]
# Arithmetic Operators: %
Modulo / remainder from integer division (operator **%**)
```java
int a = 7;
int b = 2;
System.out.println(a % b);   // 1
```
```java
System.out.println(3 % 2);   // 1
System.out.println(4 % 2);   // 0
System.out.println(3.5 % 1); // 0.5
```
[/slide]