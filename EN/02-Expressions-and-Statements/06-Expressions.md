[slide]
# Expressions
**Expressions** == sequences of operators, literals and variables which are evaluated to a value.

* Consist of at least one **operand**
* Can have 1 or more **operators**
```java
int y = x + 5;
```
```java
String name = "John Doe"
```
```java
int r = (150-20) / 2 + 5;
```
In most of the contexts in which expressions are used, for example in statements, the expression is expected to evaluate to some value. 

If x and y are integers, the expression x + y evaluates to a numeric value. 

Every value has an associated type. For example, if x and y are both variables of type int, the value of the expression x + y is also typed as int.
If the value is assigned to a variable of a different type, or if x and y are different types, they need to be converted to a certaint type.

# Priorities of arithmetic operations
The standard rule for priorities of arithmetic operations is applied: multiplying and dividing are always done before adding and subtracting. 

In case of an expression in brackets, it is calculated first.

 When two operators share an operand the operator with the higher **precedence** goes first. For example, **1 + 2 * 3** is treated as **1 + (2 * 3)**, 
 whereas **1 * 2 + 3** is treated as **(1 * 2) + 3** since multiplication has a higher precedence than addition.

[/slide]

[slide]
# Video

[vimeo-video videoId="341522009" startTimeInSeconds="7018" endTimeInSeconds="7376" /]

[/slide]