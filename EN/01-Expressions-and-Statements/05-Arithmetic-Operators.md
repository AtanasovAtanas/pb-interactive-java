[slide]
# Arithmetic Operators

# Arithmetic Operators: + and -
Arithmetic operators are used to perform **mathematical operations** like addition, subtraction, multiplication etc.

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
Dividing numbers is done using the / operator. 

It works differently with integers and floating point numbers. When we divide two integers, an integer division is 
applied, and the obtained output is without its fractional part. 

When we divide two numbers and at least one of them is a float number, a floating division is applied, and the 
obtained result is a float number, just like in math.

The integer division by 0 causes an exception during runtime, but float numbers divided by 0 do not cause an exception and 
the result is +/- infinity or a special value NaN.

When **dividing** integers, the result is also integer:
```java
int a = 25;
System.out.println(a / 4);  // Integer result: 6
System.out.println(a / 0);  // Error: division by 0
```
When **dividing floating-points**, the result is also a floating-point number and 
the division never fails, and works correctly with the special values Infinity and -Infinity:
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

Java modulo operation is used to get the reminder of a division. The basic syntax of Java Modulo is a % b. Here a is divided by b and the remainder of that division is returned.
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

[slide]
# Video

[vimeo-video videoId="341522009" startTimeInSeconds="6282" endTimeInSeconds="7007" /]

[/slide]