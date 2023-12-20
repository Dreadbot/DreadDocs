---
order: 99
---
# Command Based Programming

## What is Command Based Programming?

Command Based programming is the `design pattern` we use to link together actions and `subsystems`. We use this design pattern because it makes the code easier to write, read, and does it in less lines of code. We call actions `commands` in Java, which are all the differen things that subsystems can do.

## What is a command?

A command encodes an action that a subsystem can preform. Here is an example:  

```java

public class IntakeCommand extends CommandBase {

    private Intake intake;
    public IntakeCommand(Intake intake) {
        this.intake = intake;
    }

    @Override
    public void execute() {
        intake.intake();
    }

    @Override
    public void end(boolean interrupted) {
        intake.stopMotors();
    }
}
```
!!!info
Please reference [classes](/Java/Classes.md) for more information about inheritance
!!!

A command is split into 4 parts: The constructor, The intialize function, the execute function, and the end function.
The constructor takes in 1 argument if it is applicable, which is the subsystem that the command acts on. The intialize function is executed one time when the command is `scheduled`.    