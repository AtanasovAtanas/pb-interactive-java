[slide]
# The Switch-Case Statement
The switch-case condition works as a sequence of if-else blocks. 

Whenever the work of our program depends on the value of one variable, instead of making consecutive conditions with if-else blocks, we can use the conditional switch statement. 

It is being used for choosing between a list of possibilities. 

The statement compares a given value with defined constants and depending on the result, it takes an action.

We put the variable that we want to compare, inside the brackets after the operator switch and it is called a "selector". 

Here the type must be comparable (numbers, strings). 

Consecutively, the program starts comparing each value that is found after the case labels. 

Upon a match, the execution of the code from the respective place begins and continues until it reaches the operator break.

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