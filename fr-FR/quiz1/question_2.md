--- question ---

---
legend: Question 2 sur 3
---

Dans ton projet, tu as utilisé `Gestes`{:class='microbitinput'} pour permettre à l'utilisateur·rice de choisir son humeur.

Lequel de ces blocs de code permettrait à un utilisateur de choisir son humeur.

--- choices ---

- (x)

```microbit
input.onGesture(Gesture.TiltLeft, function () {
    humeur = 1
    basic.showIcon(IconNames.Happy)
    basic.pause(500)
    basic.showString("^")
})
```

--- feedback ---
Awesome! Lorsque l'utilisateur·rice incline son micro:bit vers la gauche, il peut choisir son humeur.
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
Ceci est une fonction pour ta réponse et ne permettra pas à l'utilisateur·trice de choisir son humeur.
--- /feedback ---

- ( )

```microbit
basic.forever(function () {
    datalogger.log(datalogger.createCV("", 0))
})
```

--- feedback ---
Ce bloc de code t'aidera à enregistrer les données provenant des entrées des capteurs sur le micro:bit.
--- /feedback ---

- ( )

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.clearScreen()
})
```

--- feedback ---
Il s'agit d'un bloc gestuel qui effacerait le contenu de l'écran du micro:bit mais ne permettrait pas à l'utilisateur de choisir son humeur.
--- /feedback ---

--- /choices ---

--- /question ---
