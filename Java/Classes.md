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

    public void turnRobotOff() {
        this.isRobotOn = false;
    }

}
```
## Modifiers
There is a lot going on here, but let's break it down.  
First, let's focus on `modifiers`. `public` and `private` before the variables, classes, and functions are `modifiers`. Modifiers allow us to give or restrict access to something. In this example, the variable `robotAge` is private, so that means only the class itself has access to it, and nothing else can read or write it. The variable `isrobotOn` however, is public, meaning any piece of code can read and write to it. 

One important clarification to make is that these are not technically variables, they are `members`, that means they act slightly differently than variables. We will touch more on it later. 

## Constructor

Next, let's talk about the `constructor`. The constructor is run whenever a new `instance` is created. This is our init "function". It looks sort of like a [Function](./Functions.md), but it doesn't have a return type, and the name of the function is capitalized and is the same name as the class.  You should put anything that needs to be initialized when a new instance is created here, such as setting up members and calling functions.

!!!info
Even though the constructor is not a function, you can still pass in input `arguments`!
See [Functions](./Functions.md) for more information.
!!!

## Dot Operator

You may have noticed that the member initialization inside the constructor looks different than a normal variable declaration. The two things in front of the variable are the `this` keyword and the member operator, or "dot" as many people call it. Let's break it down:
```java
this.robotAge = 3;
```
The `this` keyword refers to the parent class that the code is running in, so in this case, `this` means the Robot class object. Next, let's talk about the member operator, or "dot" as almost everyone calls it. It allows you to reference a member, method, or subclass that is declared within the class. On the left of the dot operator, you put the name of the object you want to reference from, and on the right, you put the name of the member, method, or subclass you want to reference. In this case, we reference the Robot class, and then we reference the `robotAge` member. This may seem redundant, but we use this to clarify which variables are arguments and which are members, allowing us to have the same named arguments as members. However, if you differently named arguments and members or no arguments at all, it is not necessary, but it is a best practice.  

## Methods

Another piece of classes we have yet to talk about are `methods`. Methods are special functions inside of classes, and they work basically the same way. however, you need to include a `modifier` for them to function properly. to call methods, you simply use the dot operator, such as:
```java
this.turnRobotOff();
```
As you can see, you call a method the same as a function, just with the dot operator and reference to a class.

## Instantiation

We have a class, now how do we use it? Classes on their own do not run their code unless they are `instantiated`, which means making a live, working copy of the "blueprint" that is the class. It's kind of like a house, the instance is the actual house and the blueprint is the class. Each instance is its own "ecosystem" of members and methods, which means that each instance can have different values for each of the different members. Such as 2 Robot instances having different values for isRobotOn. So how do we create a new instance of a class?
```java
Robot robotInstance = new Robot();
```
Whenever we make a new instance, we need to set it to a variable so that we can reference it later. You probably have also noticed that the type of the variable is `Robot`! Because we need a type for our instance, and its not one of the primitives, we need to use the class as the type, which is as simple as typing the name of the class you are instantiating. Next, let's look at the `new` keyword, this tells java we want a new instance of whatever class comes after the `new` keyword. Then we add two parentheses to call the constructor and voila! You have your very own instance.