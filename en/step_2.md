## Start up screen

You may want your mood checker to be used by your friends and family. 

This means you can create a start-up screen to show instructions on how to use your program.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
  <span style="color: #0faeb0">**User experience**</span> design is an important part of creating a product. It means thinking about ways to make your programs easy to understand and use.
</p>

### Choose your theme

--- task ---

Think about the times you've gotten back from school or from an outing.
Your family or friends might have asked how your day went. What responses have you given?

You might have said:
+ I had a good day
+ I had an okay day
+ I didn't have a good day

[Boxout about moods and mental health]

Based on the mood, you can create responses that use:

+ Text to show them a message 
+ Icons and animations to cheer them up
+ Melodies and sounds for calmness or excitement


--- /task ---

### Create your project

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org){:target="_blank"}

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app){:target="_blank"}.

--- /collapse ---

--- /task ---

Once the editor is open, you will need to create a new project and give your project a name. 

--- task ---

Click on the **New Project** button.

<img src="images/new-project-button.png" alt="The New Project button inside MakeCode." width="250"/>

--- /task ---

--- task ---

**Tip:** Give your project a helpful name that relates to the program you’re creating. This will make it easier to find if you create other projects on MakeCode.

--- /task ---


### Make your start up screen

Create a start-up screen that shows your user what your device is for and how to use it.

You should make this in the `on start`{:class='microbitbasic'} block of your new project. 

--- task ---

Add some `Basic`{:class='microbitbasic'} blocks to your `on start`{:class='microbitbasic'} block that your user will see when the program starts.

You could show an **icon**, make an **animation** or display **text**.

For instance it could show a heart.

```microbit
basic.showIcon(IconNames.Heart)
```

[[[microbit-icons]]]

[[[microbit-animation]]]

[[[microbit-text]]]

If your start-up screen is complicated you might want to organise the code into a **function**.

[[[microbit-function]]]

--- /task ---

--- task ---

Test your screen, show it to a friend and see if they know what the program does. 

--- /task ---

### Select a mood


Your program should the ask user about their day by letting them choose from set options.

--- task ---

Add instructions (using the `show string`{:class='microbitbasic'}) to the `on start`{:class='microbitbasic'} block.

The instructions should tell the user how to select each mood.

This will help the user know what gestures to use to input their mood.

[[[microbit-text]]]

Remember: scrolling text on a micro:bit takes a long time so keep your text short.

--- /task ---

--- task ---

Add icons to represent each mood.

[[[microbit-icons]]]

--- /task ---

### Choosing three moods for the day

--- task ---

You now need to add gestures for each mood. 
You need to add one gesture each to your Workspace for:
+ Good day
+ Okay day
+ Bad day

[[[microbit-gesture-trigger]]]

--- /task ---

### Create a variable

--- task ---

Create a variable called `mood`. 

[[[microbit-create-variables]]]

--- /task ---

--- task ---

Add the variable to your `gesture`{:class='microbitinput'} block.

Here is an example of the code blocks you could use:

```microbit
input.onGesture(Gesture.Shake, function () {
    mood = 0
})
```
--- /task ---

--- task ---

You will also need to use a number to represent each mood. 

For example `Good day` could be `1`
`Okay day` could be `2`
`Bad day` could be `3`

Change the `0` to `1` in your `set mood`{:class='microbitvariables'} variable to match the correct mood. 

```microbit
input.onGesture(Gesture.Shake, function () {
    mood = 1
})
```

--- /task ---

--- task ---

You could show an **icon** or an **animation** to represent each mood. You could also draw something using `show leds`{:class='microbitbasic'}

[[[microbit-icons]]]

[[[microbit-animation]]]

Your event should now look something like this (the exact blocks could look different):

```microbit
input.onGesture(Gesture.Shake, function () {
    mood = 1
    basic.showLeds(`
        # # . # #
        . . . . .
        . . # . #
        . # # # .
        . # # # .
        `)
})
```

--- /task ---

--- task ---

Repeat these steps twice so you have blocks in each gesture.

--- /task ---

--- task ---

In your `gesture`{:class='microbitinput'} block, tell the user to use an `event` to set their mood.

[[[microbit-text]]]

For a better user experience, add a `pause`{:class='microbitbasic'} block between the mood icon and the instruction block.

```microbit
input.onGesture(Gesture.Shake, function () {
    mood = 1
    basic.showLeds(`
        # # . # #
        . . . . .
        . . # . #
        . # # # .
        . # # # .
        `)
    basic.pause(100)
    basic.showString("Press A")
})
```
--- /task ---

### Test your program

--- task ---

When the simulator restarts, check that you're happy with the instructions, icons and animation for your start-up screen.

Check that when you use a gesture such as a `on tilt right`{:class='microbitinput'} block, the correct mood icon or animation is shown.

--- /task ---


