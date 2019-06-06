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