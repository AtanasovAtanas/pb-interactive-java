[slide]
# The Switch-Case Statement
Used for choosing among a list of possibilities

Alternative to an ***if-else*** statement
```java
switch (selector) {
  case value1:
    statements;
    break;
  default:
    statements;
    break;
}
```
# Print Yes/No Example
```java
String choice = scanner.nextLine();
switch (choice) {
  case "Y":
    System.out.println("Yes");
    break;
  case "N":
    System.out.println("No");
    break;
  default:
    System.out.println("Invalid response");
    break;
}
```
[/slide]

[slide]
# Multiple Labels
Same logic may apply for more than one case
```java
switch (selector) {
  case value1:
  case value2:
    statements;
    break;
  default:
    statements; 
    break;
}
```
# Example
```java
String animal = scanner.nextLine();
switch (animal) {
  case "dog":
  case "cat":
    System.out.println("mammal");
    break;
  default:
    System.out.println("unknown"); 
    break;
}
```
[/slide]