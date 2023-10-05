## Create a response

### Set your mood

Well done, you have created the moods for your user to choose from.
You will now need to use an event to trigger a response.

--- collapse ---

---
title: Why use events?
---

Events are a good choice if you want your user to interact with the program. 

For example in the karaoke mood checker, gestures were used to choose from a range of moods, and then the user presses Button A to set their choice.

--- /collapse ---


--- task ---


#### Using Events

Add any event block of your choice into your Workspace.

[[[microbit-buttons]]]

For example, in Mood animator, the `on logo pressed`{:class='microbitinput'} block is used.

--- /task ---

### Create your first response

Now you have chosen an event block, you need to program a response inside it.

--- task ---

Drag an `if`{:class='microbitlogic'} block from the `Logic`{:class='microbitlogic'} menu. 

Place it inside your event block.

In this example, the `on button`{:class='microbitinput'} block has been used.

```microbit
input.onButtonPressed(Button.A, function () {
    if (true) {
    	
    }
})
```
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

Change the `0` to `1` to the right on the `0 = 0`{:class='microbitlogic'} block.

Your blocks of code could look like this:

```microbit
input.onButtonPressed(Button.AB, function () {
    if (mood == 1) {
    	
    }
})
```

--- /task ---

--- task ---

Add a response block inside the `if`{:class='microbitlogic'} block.

You can show an icon or an animation or play some music.

[[[microbit-icons]]]
[[[microbit-animation]]]
[[[microbit-playing-sounds]]]

--- /task ---

### Test your program

--- task ---

When the simulator restarts, use a gesture to choose your mood.

Use your event to trigger your response.

[Add video to show working on micro:bit]
--- /task ---
