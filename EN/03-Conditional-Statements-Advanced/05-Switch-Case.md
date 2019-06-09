[slide]
# The Switch-Case Statement
Used for choosing among a list of possibilities

Alternative to an ***if-else*** statement if a single expression is tested against three or more conditions

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
[/slide]

[slide]
# The default case
The default case specifies the switch section to execute if the match expression doesn't match any other case label

If a default case is not present and the match expression doesn't match any other case label, program flow falls through the switch statement

The default case can appear in any order in the switch statement, but regardless of its order in the source code, it's always evaluated last, after all case labels have been evaluated

# Example
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
We can use multiple case labels, when we need to execute identical logic for different cases

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