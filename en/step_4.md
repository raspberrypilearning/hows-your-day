## Create your responses

--- task ---

Delete the existing response you placed inside the `if`{:class='microbitlogic'} block in the `on button`{:class='microbitinput'} block.

--- /task ---

--- task ---

For each mood, create a function for each response activity that will be shown to your user. 

You could create three functions for the three mooods the user can choose from.

[[[microbit-function]]]

--- /task ---

### Program your response function. 

The things you need to put inside your function will depend on what type of response you want to show to the user. 

--- task ---

Use your micro:bit skills to create your responses. 

Here are some reminders of things you have already done in the Explore projects that you might want to use.

#### Using the LEDs

[[[microbit-icons]]]

[[[microbit-animation]]]

[[[microbit-text]]]

[[[microbit-plot-graph]]]

#### Using sensors

[[[microbit-mic]]]

[[[microbit-fine-movement]]]

#### Doing cool stuff

[[[microbit-timer]]]

[[[microbit-counting]]]

[[[microbit-animation]]]

[[[microbit-making-choices]]]

[[[microbit-playing-sounds]]]

[[[microbit-mic]]]

[[[microbit-volume]]]

Have a look over the projects you have made throughout the path for inspiration for your responses.

Here is an example of responses you can add:

```microbit
input.onGesture(Gesture.TiltRight, function () {
    mood = "Bad day"
    basic.showLeds(`
        # # . # #
        . . . . .
        . . # . .
        . # # # .
        # . . . #
        `)
    basic.pause(100)
    basic.showString("Press A+B")
})
```
--- /task ---

--- task ---

From the `Advanced `section of the Toolbox, drag out a `call`{:class='microbitfunctions'} block from the `Functions`{:class='microbitfunctions'} menu.

Place it inside the `if`{:class='microbitlogic'} block in the `on button`{:class='microbitinput'} block.

--- /task ---

### Create more responses

--- task ---

Add more responses to your `on button`{:class='microbitinput'} block for the other mood options.

Click the `+` button at the bottom of your `if`{:class='microbitlogic'} block to add `else if`{:class='microbitlogic'} blocks.

[[[microbit-selection]]]

--- /task ---

--- task ---

You can also log your user's mood.

[[[microbit-datalogging]]]

--- /task ---


### Test your program

--- task ---

Test your program. 

When the simulator restarts, use a gesture to choose your mood.

Press the `Button A+B` to check the responses for each mood you choose.



--- /task ---

