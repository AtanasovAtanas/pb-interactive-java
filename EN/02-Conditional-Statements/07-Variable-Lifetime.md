[slide]
# Variable Lifetime
The scope, in which it can be used:

```java
String currentDay = "Monday"; 
if (currentDay.equals("Monday")) {
  //The variable salary exists only in the block of code of the if statement
  double salary = Double.parseDouble(sc.nextLine());
}
System.out.println(salary); // Compile-time error!
```
[/slide]