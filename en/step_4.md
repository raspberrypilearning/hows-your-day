## Create more responses

For any mood your user has chosen, you can show them something or give them an activity to do.

--- task ---

Add more responses to your `on button`{:class='microbitinput'} block for the other response options.

Click the `+` button at the bottom of your `if`{:class='microbitlogic'} block to add `else if`{:class='microbitlogic'} blocks.

[[[microbit-making-choices]]]

--- /task ---

--- task ---

Use your micro:bit skills to create more responses. 

Add them inside the `else if`{:class='microbitlogic'} blocks.

Here are some reminders of things you have already done in the Explore projects that you might want to use.

#### Using the LEDs

[[[microbit-icons]]]

[[[microbit-animation]]]

[[[microbit-text]]]

[[[microbit-plot-graph]]]

#### Using sounds

[[[microbit-playing-sounds]]]

[[[microbit-mic]]]

[[[microbit-volume]]]

#### Other

[[[microbit-timer]]]

[[[microbit-counting]]]

Have a look over the projects you have made throughout the path for inspiration for your responses.

Here is an example of responses you can add:

```microbit
input.onButtonPressed(Button.A, function () {
    if (mood == 1) {
        basic.showString("Sing!")
        music.play(music.stringPlayable("- - - - - - - - ", 120), music.PlaybackMode.UntilDone)
    } else if (mood == 2) {
        basic.showString("Dance!")
        music._playDefaultBackground(music.builtInPlayableMelody(Melodies.Dadadadum), music.PlaybackMode.UntilDone)
    } else {
        basic.showString("Move!")
        music._playDefaultBackground(music.builtInPlayableMelody(Melodies.Funk), music.PlaybackMode.InBackground)
    }
})
```
--- /task ---


### Using functions to organise your responses

For each response, you can create a function for the activity that will be shown to your user. 

This will tidy up your code if you have a lot of blocks inside each `if`{:class='microbitlogic'} and `else if`{:class='microbitlogic'} blocks.

You could create three functions for the three responses your user is shown.

--- task ---

[[[microbit-function]]]

--- /task ---

--- task ---

Drag your response blocks into your newly created function blocks. 

Here is an example code from a function block:

```microbit
function goodDay () {
    basic.clearScreen()
    basic.showString("Sing!")
    basic.pause(100)
    music.play(music.stringPlayable("C C G G A A G - ", 120), music.PlaybackMode.LoopingInBackground)
}
```

--- /task ---

You will need to call your function inside your event block to use it.

--- task ---

From the `Advanced` section of the Toolbox, drag out your `call`{:class='microbitfunctions'} blocks from the `Functions`{:class='microbitfunctions'} menu.

Ensure you use the correct response call block.

Place them inside the `if`{:class='microbitlogic'} and `else if`{:class='microbitlogic'} blocks in your event.

--- /task ---

### Reset your program

Once a user has set their mood and completed a response, you can allow them reset the program and start again.

--- task ---

From the `Input`{:class='microbitinput'} menu, drag out an event block you have not used in your project.

Place it in your workspace.

--- /task ---

--- task ---

From the `Music`{:class='microbitmusic'} menu, drag out a `stop all sounds`{:class='microbitmusic'} block.

Place it inside your event block.

The `on logo pressed`{:class='microbitinput'} block has been used in this example.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
})
```
--- /task ---

--- task ---

Duplicate your startup screen blocks or startup screen function.

Place it below the `stop all sounds`{:class='microbitmusic'} block.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
    startupScreen()
})
```

--- /task ---

### Test your program

--- task ---

When the simulator restarts, use a gesture to choose your mood.

Use your event to trigger your responses.

Use your other event block to reset the program.

--- /task ---

[[[download-to-microbit]]]

Next, it is time to check what you have learnt!