# Stream-Deck-Tools

A collection of icons and triggers I use on my Elgato Stream Deck Gen 1, running [Bitfocus Companion](https://bitfocus.io/companion).
All icons belong to their respective owners.

## Installation:

To install these tools, either recall a full system-wide backup (which is not provided here for privacy reasons.), or import sections individually (see below):

### Installing - Main Clock + Stopwatch/Timer

#### Connections

To install the main clock, you also need to have the following connections added and configured as below:

- `Generic: Button Blink` ([GitHub](https://github.com/bitfocus/companion-module-generic-blink/)) named `generic-blink`.
- `Generic: Stopwatch` ([Github]()) named `stopwatch`.
- `Generic: Stopwatch` ([Github]()) named `timer`.

#### Custom Variables:

Next, create these custom variables. Note that companion automatically adds `internal:custom_` before each variable when it is created:

- `mainClock` - Persist Value set to `False`.
- `stopwatchPaused` - Persist Value set to `True`.
- `timerRunning` - Persist Value set to `True`.

![The variables to add.](<Docs/Screenshots/Installing Main Clock Variables.png>)

#### Import Pages

After that, import the pages for the Stopwatch and Timer, by selecting the "Import / Export" option in the menu bar:
![The Import/Export Page.](<Docs/Screenshots/Import Export Page.png>)
Select "Import", and select the pages to import:

- `Pages/Stopwatch.companionconfig`
- `Pages/Timer.companionconfig`

#### Import Triggers

Finally, import the two triggers used by this tool. Again, go to the "Import / Export" page, and import the following triggers from the Triggers folder in this project.

- `Triggers/Main Clock.companionconfig`
- `Triggers/Timer Alarm.companionconfig`

#### Configuration

Most of the configuration should remain the same, however the one thing that you will likely have to change is in the trigger for the timer.

Open the triggers page, and select the timer alarm.
![The trigger settings that can be changed.](<Docs/Screenshots/Configuring Timer Alarm Trigger.png>)

Change the page (`21` in this example) and button (`21/2/4`), by replacing the `21` with the page you imported the timer to.

## Next Steps:

- Re-write the "Main Clock" trigger to support a third input (and potentially more), to allow for more data to be displayed.
- Add another trigger I've written, which allows for the creation of a Shift key, where the function and appearance of a button can be changed whist holding any "Shift" key.
