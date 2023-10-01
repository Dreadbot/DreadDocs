---
order: 97
---

# Classes

`Classes` are one of the most important features of Java. They allow us to represent and package code in a way that is easy and convient to reuse.  
Lets look at an example:
```java
public class Robot {

    private int robotAge;
    public boolean isRobotOn = false;

    public Robot() {
        this.robotAge = 3;
        this.isRobotOn = true;
    }

}
```

There is a lot going on here, but lets break it down.  
First, lets focus on `modifiers`. `public` and `private` before the variables, classes, and functions are `modifiers`. Modifiers allow us to give or restrict access to something. In this example, the variable `robotAge` is private, so that means only the class itself has access to it, and nothing else can read or write it. The variable `isrobotOn` however, is public, meaning any piece of code can read and write to it.  

One important clairification to make is that these are not technically variables, they are `members`, that means they act slightly differently than variables. We will touch more on it later.