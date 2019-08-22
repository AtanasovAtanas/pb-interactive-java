[slide]
# Infinite While Loop
Repeating a block of code an **infinite number of times**

Infinite ***while*** loops are caused when the check condition is always evaluated to ***true***

```java
while(true) {
  // Commands
}
```

# Example: Infinite While Loop (Bug)

```java
String command = "Add";
while (!command.equals("End")) {
  System.out.println("Executing: " + command);
}
```

# Example: Finite Loop (Bug Fixed)

```java
Scanner scanner = new Scanner(System.in);

String command = "Add";
while (!command.equals("End")) {
  System.out.println("Executing: " + command);

  command = scanner.nextLine();
}
```
[/slide]