# Stream-Deck-Tools
A collection of icons and triggers I use on my Elgato Stream Deck Gen 1, running [Bitfocus Companion](https://bitfocus.io/companion).
All icons belong to their relative owners.

## Trigger - Main Clock
A trigger which takes in the current system time, and a [Stopwatch Connection](https://github.com/bitfocus/companion-module-generic-stopwatch), and stores one into a custom variable, to be displayed on any buttons. By default, the trigger returns the system clock when the stopwatch is not running, and shows the stopwatch count when it is running:

| Image | Example |
| --- | --- |
| ![The system time, shown on an example button](demos/main-clock/main-clock.png?raw=true "System Time") | The current system time being displayed on an example button. |
| ![The stopwatch timer, shown on an example button](demos/main-clock/stopwatch.png?raw=true "Stopwatch") | The stopwatch readout, shown on an example button. |

This is done using an expression, to perform a ternary comparison, which sets the output variable to either the system time, or the stopwatch readout.

![The expression used to return the output](demos/main-clock/expression.png?rwa=true "Expression")

## Next Steps:
- Re-write the "Main Clock" trigger to support a third input (and potentially more), to allow for more data to be displayed.
- Add another trigger I've written, which allows for the creation of a Shift key, where the function and appearance of a button can be changed whist holding any "Shift" key.