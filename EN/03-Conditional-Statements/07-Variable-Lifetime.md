[slide]
# Variable Lifetime
Each variable has a range in which it exists, called variable scope
  * The range specifies where a variable can be used and how long is its lifetime

In the **Java language**, the scope in which a variable exists, starts from the line in which we defined it and ends with the first closing curly bracket (of the method, the if statement, etc.).

In the example below, on the last line we are trying to print the variable salary that is defined in the if statement, we will get an error because we don't have access to it:
```java
String currentDay = "Monday"; 
if (currentDay.equals("Monday")) {
  //The variable salary exists only in the block of code of the if statement
  double salary = Double.parseDouble(sc.nextLine());
}
System.out.println(salary); // Compile-time error!
```
[/slide]

[slide]
# Video

[vimeo-video videoId="341539841" startTimeInSeconds="4005" endTimeInSeconds="4209" /]

[/slide]