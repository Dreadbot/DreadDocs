---
order: 98
---

# Functions
A `Function` is a way of packaging code so that we can reuse it. A function can have inputs and outputs, so they can be quite a useful tool in Java programming.

Here is a simple example:   
```java
boolean robotIsOn = false;

void turnRobotOn() {
    robotIsOn = true;
}

turnRobotOn();
```
There is a lot going on here but we will focus on the function declaration.
to declare a function, we simply need a type and a name. The type tells us what the function will return, in this case that is `void`, which is nothing. The name of the function is how we reference it. After the name comes the parentheses, which hold the `paramters` of the function, we will go into depth about parameters later. In this case there are no parameters, so it's just the parentheses. Lastly, we have the curly brackets. These tell Java where the code for the function starts and ends.

## Parameters and Returns

Sometimes, we want a function to do something based on an input, and give an output. Thats where `parameters` and `returns` come in.
Here is an example of parameters and returns

```java
int addTwoNumbers(int a, int b) {
    return a + b;
}
int result = addTwoNumbers(3, 4);
```

To add parameters to a function, simply give the parameter a type and a name and add a comma in between each parameter.
you can user parameters as a kind of local variable that only exists inside the function declaration. To return something from a function, use the `return` keyword. You can pass either a variable or an expression (as we have in this case). Notice how we changed the functions type to reflect what we are returning.  
To call any function, just write the name with a pair of parentheses in which you add any parameters the function has.  
For more information on types when working with functions, check out [Types](./Types.md)