
--- question ---

---
legend: Question 2 of 3
---

In your project you used `Gestures`{:class='microbitinput'}, to allow the user to choose their mood. 

Which of these code blocks would allow a user to choose their mood.

--- choices ---

- (x) 

```microbit
input.onGesture(Gesture.TiltLeft, function () {
    mood = 1
    basic.showIcon(IconNames.Happy)
    basic.pause(500)
    basic.showString("^")
})
```

  --- feedback ---
Awesome! When the user tilts their micro:bit to the left they're able to choose their mood.
  --- /feedback ---

- ( ) 

 
```microbit
function badDay () {
    basic.clearScreen()
    basic.showString("Sing along!")
    basic.pause(100)
}
```

  --- feedback ---
This is a function for your response and will not allow the user choose their mood.
  --- /feedback ---

- ( ) 

```microbit
basic.forever(function () {
    datalogger.log(datalogger.createCV("", 0))
})
```

  --- feedback ---
This block of code would help you log data from the sensor inputs on the micro:bit.
  --- /feedback ---

- ( ) 

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.clearScreen()
})
```

  --- feedback ---
This is a gesture block that would clear the screen of the micro:bit but won't let the user choose their mood.
  --- /feedback ---

--- /choices ---

--- /question ---
