---
order: 94
---

# Types

## What Are types?

Java is a `statically typed` langauge. This means that we have to work with `types`. `Types` are how we tell Java what something **is** or **returns**.  
In [variables](./Variables.md), we looked at this example:
```java
boolean isRobotOn = false;
```
Here, we tell java what the data that the variable contains is. In this case, the variable `isRobotOn` is of type `boolean`.

In [functions](./Functions.md), we looked at this example:
```java
int addTwoNumbers(int a, int b) {
    return a + b;
}
```
In this example, we tell Java what this function will **return**, this allows us to guarantee* that we will get a return value of type `int`. This allows has the side effect of being able to use `Code Completion` on a lot more objects and variables that we would be able to otherwise.  
\* This is true for about 99% of cases

## Primitives

So far, all the types we have been looking at have been `primitives`. A `primitive` is a type that Java supplies us by default. You can tell which types are primitives as primitives always start with a lowercase.  
Here are some primitives:

Name | Meaning
--- | ---
`int` | Integers (1, 2, 3, etc.)
`byte` | A number from 0 to 255
`short` | A number from -32768 to 32767
`long` | A number from -2147483648 to 2147483647
`float` |  A fracional number that goes up to 7 decimal places (1.234, etc.)
`double` | A fracional number that goes up to 15 decimal places
`boolean` | A true or false value
`char` | A single character

## Other Types

So far, we have only looked at primitives, but Java has more to offer then that! We are going to look at `non-primitive` data types. You can tell if a type is not a primitive if it starts with an uppercase.

For example:
```java
MyType myVariable = new MyType();
```
How do we create types? Its super simple! We simply use the class name of the class we are instantiating as the type.  
For more information about instantiating classes, check out [classes](./Classes.md).