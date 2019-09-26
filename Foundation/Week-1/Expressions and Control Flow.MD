# W01 - D04 - Expressions and Control Flow
***made by [Gergo](https://github.com/vjanosigergely)***

- [Basic Types (primitives)](#basic-types-primitives)
- [Declaring Variables](#declaring-variables)
    - [Casting (=changing data types)*](#casting-changing-data-types)
    - [Strings](#strings)
        - [Concatenation](#concatenation)
- [Operators](#operators)
    - [Arithmetic operators](#arithmetic-operators)
    - [Comparison operators](#comparison-operators)
    - [Logical operators](#logical-operators)
- [Conditional Statements](#conditional-statements)
    - [if - else if - else](#if---else-if---else)
    - [Switch](#switch)
- [Loops](#loops)
    - [While Loop](#while-loop)
    - [Do While Loop](#do-while-loop)
    - [For Loop](#for-loop)
        - [Fori](#fori)
        - [Nested For Loop ](#nested-for-loop )
- [User Input](#user-input)
- [IntelIJ Shortcuts for Java](#intelij-shortcuts-for-java)
- [Breaking Lines](#breaking-lines)

## Basic Types (primitives)
| Type          | Size (bits) |     Minimum      |                Maximum                 |            Example            |
|:-------------:| -----------:| ---------------: | --------------------------------------:|:----------------------------- |
|     `byte`    |      8      |    -2<sup>7</sup>|                         2<sup>7</sup>-1|                `byte b = 100;`|
|    `short`    |     16      |   -2<sup>15</sup>|                        2<sup>15</sup>-1|             `short s = 30000;`|
|      `int`    |     32      |   -2<sup>31</sup>|                        2<sup>31</sup>-1|           `int i = 100000000;`|
|     `long`    |     64      |   -2<sup>63</sup>|                        2<sup>63</sup>-1|    `long l = 100000000000000;`|
|    `float`    |     32      | -2<sup>-149</sup>| (2 - 2<sup>-23</sup>) * 2<sup>127</sup>|            `float f = 1.456f;`|
|   `double`    |     64      |-2<sup>-1074</sup>|(2 - 2<sup>-52</sup>) * 2<sup>1023</sup>|`double f = 1.456789012345678;`|
|     `char`    |     16      |        0         |                        2<sup>16</sup>-1|`char c = ‘c';`                |
|  `boolean`    |      1      |        -         |                   -                    |`boolean b = true;`            |



## Declaring Variables
|   type|     name   |assigning|value|semicolon|
| -----:|:---------- |:-------:|:---:|:------- |
|  `int`| `myNumber` |      `=`|  `5`|      `;`|
`int myNumber = 5;`

****

### Casting *(=changing data types)* 
- `double myDouble = 9.78;`	-> outputs 9,78
- `int myInt = (int) myDouble;` -> outputs 9

****

### Strings		
|    type|   name   |assigning|    value|semicolon|
|:------:|:--------:|:-------:|:-------:|:-------:|
|`String`|`greeting`|      `=`|`"Hello"`|      `;`|
`String greeting = "Hello";`
> - **Capital S** <br/>
> - **assign value using “ “**

#### Concatenation
```java
    String firstName = "John";
    String lastName = "Doe";
    System.out.println(firstName + " " + lastName);
```

****

## Operators
### Arithmetic Operators
|Operator|      Name    |              Description             |Example|
|:------:|:------------:|:------------------------------------:|:-----:|
|     `+`|      Addition|              Adds together two values|`x + y`|
|     `-`|   Subtraction|      Subtracts one value from another|`x - y`|
|     `*`|Multiplication|                 Multiplies two values|`x * y`|
|     `/`|      Division|        Divides one value from another|`x / y`|
|     `%`|       Modulus|        Returns the division remainder|`x % y`|
|    `++`|     Increment|Increases the value of a variable by 1|  `x++`|
|    `--`|     Decrement|Decreases the value of a variable by 1|  `x--`|

> ***The `+` operator works differently on strings and numbers***
```java
    int x = 10;
    int y = 20;
    int z = x + y;
    // z will be 30 (an integer/number)

    String a = "10";
    String b = "20";
    String c = a + b;
    // String c = a + b;   // c will be 1020 (as String)
```

****

### Comparison Operators
|Operator|                    Name| Example|
|:------:|:----------------------:|:------:|
|    `==`|                Equal to|`x == y`|
|    `!=`|               Not equal|`x != y`|
|     `>`|            Greater than| `x > y`|
|     `<`|               Less than| `x < y`|
|    `>=`|Greater than or equal to|`x >= y`|
|    `<=`|   Less than or equal to|`x <= y`|

****

### Logical Operators
|Operator|         Name|                                            Description|             Example|
|:------:|:-----------:|:-----------------------------------------------------:|:------------------:|
|    `&&`|Logical `and`|               Returns true if both statements are true|  `x < 5 &&  x < 10`|
|    `||`| Logical `or`|          Returns true if one of the statements is true|    `x < 5 || x < 4`|
|     `!`|Logical `not`|Reverse the result, returns false if the result is true|`!(x < 5 && x < 10)`|

## Conditional Statements
### if - else if - else
```java
    if (condition) {
      // block of code to be executed if the condition is true
    }
//====================================================================================
    if (condition) {
      // block of code to be executed if the condition is true
    } else {
      // block of code to be executed if the condition is false
    }
//====================================================================================
    if (condition1) {
      // block of code to be executed if condition1 is true
    } else if (condition2) {
      // block of code to be executed if the condition1 false and condition2 is true
    } else {
      // block of code to be executed if both conditions are false
    }
```

****

### Switch

```java
    // Use switch to specify many alternative blocks of code to be executed
    switch (expression) {
      case x:
        // code block
        break;          // -> breaks out of the block
                        //    Not mandatory, but saves time
      case y:
        // code block
        break;
      default:          // -> code to run if no case matches
        // code block
    }
```

## Loops
### While Loop
> ***The while loop loops through a block of code as long as a specified condition is true.***

```java
    while (condition) {
      // while the condition is true
      // code block to be executed
    }
```

****

### Do While Loop
> ***Same as While, but always executes the code block once first.***

```java
    do {
      // code block to be executed
    }
    while (condition);
```

****

### For Loop
> ***Use this when you know exactly how many times you need to loop through a block.***

```java
    for (statement 1; statement 2; statement 3) {
      // code block to be executed
    }
```

- *Statement 1* is executed (one time) before the execution of the code block.
- *Statement 2* defines the condition for executing the code block.
- *Statement 3* is executed (every time) after the code block has been executed.

#### Fori
```java
    for (int i = 0; i < n; i++) {
      // code block to be executed
    }
```

****

#### Nested For Loop 
```java
    for (int i = 0; i < n; i++) {
      for (int j = 0; j < m; j++) {
        // code block to be executed
      }
    }
```

## User Input
> ***Need to `import java.util.Scanner;`***
	
```java
    Scanner scanner = new Scanner(System.in);
    int n = scanner.nextInt();
```

## IntelIJ Shortcuts for Java
- psvm  = `public static void main(String[] args) {}`
- sout  = `System.out.println();`

## Breaking Lines
- `\n`
- `System.out.println();` always breaks line after printing
- `System.out.print();` doesn't
