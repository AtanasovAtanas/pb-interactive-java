[slide]
# The break Operator
Used for prematurely exiting the loop

Can only be executed from the loop's body

When break is executed, the code inside the loop's body after it is skipped (does not execute)

```java
Scanner scanner = new Scanner(System.in);

while (true) {
  int number = Integer.parseInt(scanner.nextLine());
  if (number % 2 != 0) {
    break;
  }
  
  System.out.println("Enter an even number!");
}
```
# Example
Sum numbers until 0 is entered
```java
Scanner scanner = new Scanner(System.in);
long sum = 0;

while (true) {
  int nextNum = Integer.parseInt(scanner.nextLine());
  if (nextNum == 0) {
      // The last number was reached
      break;
  }
  sum += nextNum;
  System.out.println("Sum: " + sum);
}
```
[/slide]
