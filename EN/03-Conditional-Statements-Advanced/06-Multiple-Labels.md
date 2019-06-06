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