--- question ---

---

legend: Vraag 2 van 3
---

In je project heb je `Gebaren`{:class='microbitinput'} gebruikt om de gebruiker zijn stemming te laten kiezen.

Met welke van deze codeblokken kan een gebruiker zijn stemming kiezen.

--- choices ---

- (x)

```microbit
input.onGesture(Gesture.TiltLeft, function () {
    stemming = 1
    basic.showIcon(IconNames.Happy)
    basic.pause(500)
    basic.showString("^")
})
```

--- feedback ---
Awesome! Wanneer de gebruiker zijn micro:bit naar links kantelt, kan hij zijn stemming kiezen.
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
Dit is een functie voor je antwoord en laat de gebruiker niet zijn stemming kiezen.
--- /feedback ---

- ( )

```microbit
basic.forever(function () {
    datalogger.log(datalogger.createCV("", 0))
})
```

--- feedback ---
Dit blok code helpt je om gegevens van de sensoringangen op de micro:bit te registreren.
--- /feedback ---

- ( )

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.clearScreen()
})
```

--- feedback ---
Dit is een gebarenblok dat het scherm van de micro:bit leegmaakt, maar de gebruiker zijn stemming niet laat kiezen.
--- /feedback ---

--- /choices ---

--- /question ---
