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

This will tidy up your code if you have a lot of blocks inside each `if`{:class='microbitlogic'} and `else if`{:class='microbitlogic'} block.

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
    basic.showString("Sing along!")
    basic.pause(100)
    music.play(music.createSoundExpression(
    WaveShape.Noise,
    500,
    499,
    255,
    0,
    3307,
    SoundExpressionEffect.None,
    InterpolationCurve.Linear
    ), music.PlaybackMode.UntilDone)
    if (input.soundLevel() > 128) {
        datalogger.log(datalogger.createCV("Sound Level", input.soundLevel()))
    } else {
        basic.showString("Sing louder!")
    }
}
```

--- /task ---

You will need to call your function inside your event block to use it.

--- task ---

From the `Advanced` section of the Toolbox, drag out your `call`{:class='microbitfunctions'} block from the `Functions`{:class='microbitfunctions'} menu.

Ensure you use the correct response call block.

Place it inside the `if`{:class='microbitlogic'} block in your event block.

```microbit
input.onButtonPressed(Button.A, function () {
    if (mood == 1) {
        goodDay()
    } else if (mood == 2) {
        okayDay()
    } else {
        badDay()
    }
})
```

Repeat this step for your `else if`{:class='microbitlogic'} blocks.

--- /task ---

### Test your program

--- task ---

When the simulator restarts, use a gesture to choose your mood.

Use your event to trigger your responses.


--- /task ---

[[[download-to-microbit]]]

Next, it is time to check what you have learnt!