---
order: 96
---
# Flow Control
`Flow Control` is the way your program can make decisions while its running. Let's look at an example!

```java

boolean isRobotOn = true; 
if (isRobotOn) {
    System.out.println('Robot is on!');
}

``` 

This is an `if` statement, and the code inside the block is only ran if the expression resolves to `boolean` value that is true. Because the expression of `isRobotOn` resolves to true, the code inside the if statement block is ran, printing out "Robot is on!" to the console.  
Let's look at some other expressions:
```java
boolean isRobotOn = false;
int robotAge = 4;
if (!isRobotOn) {
    System.out.println('Robot is off!');
}

if (robotAge == 4) {
    System.out.println('Robot age is 4!');
}

```
Here, we can see the `not` operator and the `equals` operator. The not operator resolves to the inverse of the boolean value that comes after it, so because `isRobotOn` is false, its is inverted to true, so the code inside the block is ran. The equals operator resolves to true only if both side of the operator are equivelent to each other.  

What if you wanted to do something if the if statement failed?
You would use an `if else` block!
Here is an example of one:

```java

boolean isRobotOn = false;

if (isRobotOn) {
    System.out.println('Robot is on. Yay!');
} else {
    isRobotOn = true;
}

```

Here we can see the use of a new keyword, `else`, which sits right after the closing curly bracket of the if statement and is followed by another code block. This code block is only ran if the if statement doesn't activate (such as the expression resolving to false). But wait, Theres more! You can also check for another condtion if the if statement fails by using an `else if` block!

```java
boolean isRobotOn = false;
int robotAge = 4;
if (isRobotOn) {
    System.out.println('Robot is on. Yay!');
} else if (robotAge == 4) {
    System.out.println('Robot is 4 years old!');
}

```

# Operators 
Before we get to the table, we need to talk about the difference between a `unary` and a `binary` operator.
A `unary` operator only operates on one value, and the value usally proceeds the operator (such as `!isRobotOn`).
A `binary` operator operates on 2 values, one on the left hand side of the operator and one on the right hand side (such as `2 + 2`);
Given that, here is a table of the different types of boolean operators:

Operator | Name | Meaning
--- | --- | ---
`==` | Equals | Resolves to true only if both sides of operator are equivelent
`>` | Greater than | Resolves to true only if left side is greater than the right side
`<` | Less than | Resolves to true only if left side is less than the right side
`>=` | Greater or equal than | Resolves to true only if the left side is greater than or equal to the right side
`<=` | Less or equal than | Resolves to true only if the left side is less than or equal to the right side
`&&` | And | Resolves to true only if the left side resolves to true and the right side resolves to true
`||` | Or | Resolves to true if the left side resolves to true or the right side resolves to true.
`!` | Not | Resolves to the inverse the value given