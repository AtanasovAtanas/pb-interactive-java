[slide]
# Problem: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a triangle area:

  * Read from input a side **a** and height for that side **ha**
  * Calculate the area of a triangle by the side and height
  * Print the **area**, formatted to the **2nd digit** after decimal point
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5<br>10|25,00 | 
[/slide]

[slide]
# Solution: Area of Triangle
[code-task title="Area of Triangle" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
    {
      double a = Double.parseDouble(scanner.nextLine());
      double h = Double.parseDouble(scanner.nextLine());
      double area = (a * h) / 2;
      System.out.printf("%.2f", area);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a triangle area:

  * Read from input a side **a** and height for that side **ha**
  * Calculate the area of a triangle by the side and height
  * Print the **area**, formatted to the **2nd digit** after decimal point
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5<br>10|25,00 | 
[/slide]

[slide]
# Problem: Four Operations
[code-task title="Four Operations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * **Reads** 2 real numbers from the **console**
  * Performs **4 arithmetic operations** on the obtained 2 numbers, in the following order: **+, -, *, /**
  * **Formats** and **prints** the results like this example:

[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5<br>10|5 + 10 = 15<br>5 - 10 = -5<br>5 * 10 = 50<br>5 / 10 = 0.5| 
[/slide]

[slide]
# Solution: Four Operations
[code-task title="Four Operations" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      double num1 = Double.parseDouble(scanner.nextLine());
      double num2 = Double.parseDouble(scanner.nextLine());
      System.out.printf("%f + %f = %f%n", num1, num2, num1 + num2);
      System.out.printf("%f - %f = %f%n", num1, num2, num1 - num2);
      System.out.printf("%f * %f = %f%n", num1, num2, num1 * num2);
      System.out.printf("%f / %f = %f%n", num1, num2, num1 / num2);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * **Reads** 2 real numbers from the **console**
  * Performs **4 arithmetic operations** on the obtained 2 numbers, in the following order: **+, -, *, /**
  * **Formats** and **prints** the results like this example:
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|5<br>10|5 + 10 = 15<br>5 - 10 = -5<br>5 * 10 = 50<br>5 / 10 = 0.5| 
[/slide]

[slide]
# Problem: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from days to minutes:

  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Solution: Days to Minutes
[code-task title="Days to Minutes" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      int days = Integer.parseInt(scanner.nextLine());
      int hours = days * 24;
      int minutes = hours * 60;
      System.out.println(minutes);
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from days to minutes:

  * Read a single **integer** (the **days** to be converted)
  * Convert the days to minutes (use calculations)
  * Print the **minutes**
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|2|2880|
|5|7200|
[/slide]

[slide]
# Problem: Currency Converter
[code-task title="Currency Converter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from USD to EUR:

  * Read a **floating-point number**: the **dollars** to be converted 
  * Convert dollars to euro (use fixed rate of dollars to euro: **0.88**)
  * Print the converted value in **euro**
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Solution: Currency Converter
[code-task title="Currency Converter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      double dollars = Double.parseDouble(scanner.nextLine());
      double euros = dollars * 0.88; 
      System.out.println(euros);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the speed by time and distance:

  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|17|14.96| 
|87|76.56|
[/slide]

[slide]
# Problem: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a circle area and perimeter:

  * Read a floating-point number: the radius of a circle
  * Calculate the area and perimeter of a circle
  * Print the calculated values
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.9380400259<br>Perimeter = 43.9822971502571|
[/slide]

[slide]
# Solution: Circle Area and Perimeter
[code-task title="Circle Area and Perimeter" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      double radius = Double.parseDouble(scanner.nextLine());
      double area = radius * radius * Math.PI;
      double perimeter = 2 * Math.PI * radius;
      System.out.printf("Area = %f%n", area);
      System.out.printf("Perimeter = %f%n", perimeter);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate a circle area and perimeter:

  * Read a floating-point number: the radius of a circle
  * Calculate the area and perimeter of a circle
  * Print the calculated values
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|7|Area = 153.9380400259<br>Perimeter = 43.9822971502571|
[/slide]

[slide]
# Problem: Inches to Centimeters
[code-task title="Inches to Centimeters" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from inches to centimeters:

  * Read a floating-point number: the **inches** to be converted
  * Convert the inches to **centimeters** (find the formula in Internet)
  * Print the result 
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|21|53.34| 
|71|180.34|
[/slide]

[slide]
# Solution: Inches to Centimeters
[code-task title="Inches to Centimeters" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      double inches = Double.parseDouble(scanner.nextLine());
      double centimeters = inches * 2.54;
      System.out.println(centimeters);
    }
}
```
[/code-editor]
[task-description]
Write a program to convert from inches to centimeters:

  * Read a floating-point number: the **inches** to be converted
  * Convert the inches to **centimeters** (find the formula in Internet)
  * Print the result 
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|21|53.34 | 
|71|180.34|
[/slide]

[slide]
# Problem: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
    // Write code here
  }
}
```
[/code-editor]
[task-description]
Write a program to calculate the speed by time and distance:

  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15<br>2|7.5| 
[/slide]

[slide]
# Solution: Calculate Speed
[code-task title="Calculate Speed" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      double distance = Double.parseDouble(scanner.nextLine());
      double time = Double.parseDouble(scanner.nextLine());
      double speed = distance / time;
      System.out.println(speed);
    }
}
```
[/code-editor]
[task-description]
Write a program to calculate the speed by time and distance:

  * Read 2 floating-point numbers: distance and time
  * Calculate the speed needed to travel a given distance for given time
  * Print the calculated result
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|15<br>2|7.5| 
[/slide]


[slide]
# Problem: Person Info
[code-task title="Person Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads 4 lines of **strings**: first name, last name, country and town 
  * Prints information about a person in the following format: "**{firstName} {lastName} from {country} - {town}!**"
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Kelly<br>Smith<br>Ireland<br>Cork|Kelly Smith from Ireland - Cork!|
[/slide]

[slide]
# Solution: Person Info
[code-task title="Person Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      String firstName = scanner.nextLine();
      String lastName = scanner.nextLine();
      String country = scanner.nextLine();
      String town = scanner.nextLine();
      System.out.printf("%s %s from %s - %s!",   firstName, lastName, country, town);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads 4 lines of **strings**: first name, last name, country and town 
  * Prints information about a person in the following format: "**{firstName} {lastName} from {country} - {town}!**"
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Kelly<br>Smith<br>Ireland<br>Cork|Kelly Smith from Ireland - Cork!|
[/slide]

[slide]
# Problem: Town Info
[code-task title="Town Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      // Write code here
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads **3 lines** of input: **name** (string), **population** and **area** (integers)
  * Prints information about a town in the following format: "**Town {name} has population of {population} and area {area} square km.**"
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin<br>3675000<br>984|Town Berlin has population of 3675000 and area 984 square km.|
[/slide]

[slide]
# Solution: Town Info
[code-task title="Town Info" executionStrategy="java-code" requiresInput]
[code-editor language=java]
```

public class Program
{
  public static void main(String[] args) {
      String townName = scanner.nextLine();
      int population = Integer.parseInt(scanner.nextLine());
      int area = Integer.parseInt(scanner.nextLine()); 
      System.out.printf("Town %s has population of %d and area %d  square km.", townName, population, area);
    }
}
```
[/code-editor]
[task-description]
Write a program, which:

  * Reads **3 lines** of input: **name** (string), **population** and **area** (integers)
  * Prints information about a town in the following format: "**Town {name} has population of {population} and area {area} square km.**"
[/task-description]
[code-io /]
[/code-task]

## Sample Input and Output

|       Input       | Output |
|-------------------|--------|
|Berlin<br>3675000<br>984|Town Berlin has population of 3675000 and area 984 square km.|
[/slide]