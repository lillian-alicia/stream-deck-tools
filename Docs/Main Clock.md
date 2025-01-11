## Trigger - Main Clock

A trigger which takes in the current system time, and a [Stopwatch Connection](https://github.com/bitfocus/companion-module-generic-stopwatch), and stores one into a custom variable, to be displayed on any buttons. By default, the trigger returns the system clock when the stopwatch is not running, and shows the stopwatch count when it is running:

| Image                                                                                          | Example                                                       |
| ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| ![The system time, shown on an example button](Demos/main-clock/main-clock.png "System Time")  | The current system time being displayed on an example button. |
| ![The stopwatch timer, shown on an example button](Demos/main-clock/stopwatch.png "Stopwatch") | The stopwatch readout, shown on an example button.            |

This is done using an expression, to perform a ternary comparison, which sets the output variable to either the system time, or the stopwatch readout.

![The expression used to return the output](Demos/main-clock/expression.png "Expression")
