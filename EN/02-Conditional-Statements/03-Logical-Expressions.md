[slide]
# Comparison Operators
|Operators|Designation|
|---------|-----------|
|Equal value (and type)|== (===)|
|Not equal value (and type)|!= (!==)|
|Greater than|>|
|Greater than or equal to|>=|
|Less than|<|
|Less than or equal to|<=|

[/slide]

[slide]
# Value Comparison
In programming we can **compare** values

  * The result of the logical expressions is either ***true*** or ***false***

Comparison operators can be used to construct expressions that compare the values of numeric variables. These expressions return a **boolean** value based on whether the comparison is true or false. 

Examples of such an expression are as follows.

```java
int a = 5;
int b = 10;
System.out.println(a < b);        // true
System.out.println(a > 100);      // false
System.out.println(a <= 5);       // true
System.out.println(b == 2 * a);   // true 
```
You can also compare numeric expressions. The expressions you compare can themselves be complex expressions, as in the following example.
```java
x / 45 * (y +17) >= Math.sqrt(z) / (p - (x * 16))
```
The preceding complex expression includes literals, variables, and function calls. 

The expressions on both sides of the comparison operator are evaluated, and the resulting values are then compared using the >= comparison operator. 

If the value of the expression on the left side is greater than or equal to the value of the expression on the right, the entire expression evaluates to True; otherwise,it evaluates to False.

[/slide]

[slide]
# String Comparison
Comparing text using the keyword (**equals**). The java string equals() method compares the two given strings based on the content of the string. 

If any character is not matched, it returns **false**. 

```java
String a = "Example";
String b = "Example2";
System.out.println(a.equals.(b));   // false
```

If all characters are matched or both of them are **null**, it returns **true**.

```java
String a = "Example";
String b = a;
System.out.println(a.equals.(b));   // true
```
```java
String a = "5";
String b = "5";
System.out.println(a.equals.(b));   // true 
```
[/slide]

[slide]
# Video

[vimeo-video videoId="341539841" startTimeInSeconds="1628" endTimeInSeconds="2292" /]

[/slide]