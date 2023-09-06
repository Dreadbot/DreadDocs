---
order: 95
---

# Types

## What are types?

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