[slide]
# Infinite While Loops
Repeating a block of code an **infinite number of times**

Infinite ***while*** loops are caused when the check condition is always evaluated to ***true***

```java
while (true) {
  // Commands
}
```

# Example: Infinite While Loop (Bug)
```java
String command = scanner.nextLine();

while (!command.equals("End")) {
   System.out.println("Executing: " + command);
}
```

# Example: Finite Loop (Bug Fixed)
```java
String command = scanner.nextLine()
while (!command.equals("End")) {
   System.out.println("Executing: " + command);
   
   command = scanner.nextLine();
}
```

# Example: Finite Loop with Break
```java
String command = scanner.nextLine()
while (!command.equals("End")) {
   System.out.println("Executing: " + command);

   command = scanner.nextLine();
}
```

# Example: Infinite Loop with Break
```java
while (true) {
  String command = scanner.nextLine();
  if (command.equals("End")) {
    break;
  }

  System.out.println("Executing: " + command);
}
```
[/slide]
