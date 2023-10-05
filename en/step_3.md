## Trigger response
Well done, you have created the moods for your user to choose from.
You will now need to provide a response (and log the mood) using an event. 

--- task ---

In your `gesture`{:class='microbitinput'} block, add an instruction to tell the user to press the A+B button.

This will begin the response .

[[[microbit-text]]]

--- /task ---

--- task ---

For a better user experience, add a `pause`{:class='microbitbasic'} block between the mood icon and the instruction block.

--- /task ---

--- task ---

### Using events

--- collapse ---

---
title: Why use events?
---

Events are a good choice if you want your user to interact with the program. ![Add more info here after examples]

--- /collapse ---

#### Events

[[[microbit-making-choices]]]

[[[microbit-button-trigger]]]

Add the block you need into your Workspace.

--- /task ---

### Add in some Logic

Now you have told your user to press the `Button A+B`, you need to program what happens when they do.

--- task ---

Drag an `if`{:class='microbitlogic'} block from the `Logic`{:class='microbitlogic'} menu. 

Place it inside the event `on button`{:class='microbitinput'} block.

--- /task ---

--- task ---

Open the `Logic`{:class='microbitlogic'} menu and grab the `0 = 0`{:class='microbitlogic'} block. 

Place it inside the `true`{:class='microbitlogic'} part of the `if`{:class='microbitlogic'} statement.

--- /task ---

--- task ---

Drag your `mood`{:class='microbitvariables'} variable block.

Place it inside the `0` to the left on the `0 = 0`{:class='microbitlogic'} block.

--- /task ---

--- task ---

From the `Advanced` section of the Toolbox, drag out an empty text block from the `Text`{:class='microbittext'} menu.

Place it inside the `0` to the right on the `0 = 0`{:class='microbitlogic'} block.

Type in the matching mood for `Having a good day`

Your blocks of code could look like this:

```microbit
input.onButtonPressed(Button.AB, function () {
    if (mood == "Good day") {
    	
    }
})
```

--- /task ---

--- task ---
Add a response block inside the `if`{:class='microbitlogic'} block to test your program so far.

You can show an icon or an animation or play some music.

[[[microbit-icons]]]
[[[microbit-animation]]]
[[[microbit-playing-sounds]]]

--- /task ---

### Test your program

--- task ---

Test your program. 

When the simulator restarts, use a gesture to choose your mood.

Press the `Button A+B` to show the user the response activity you created in the first `if`{:class='microbitlogic'} block.

--- /task ---
