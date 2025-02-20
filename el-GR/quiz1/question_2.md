--- question ---

---
legend: Ερώτηση 2 από 3
---

Στο έργο σου χρησιμοποίησες τις `Χειρονομίες`{:class='microbitinput'} για να επιτρέψεις στο χρήστη να επιλέξει τη διάθεσή του.

Ποιο από αυτά τα μπλοκ κώδικα θα επέτρεπε σε έναν χρήστη να επιλέξει τη διάθεσή του.

--- choices ---

- (x)

```microbit
input.onGesture(Gesture.TiltLeft, function () {
    διάθεση = 1
    basic.showIcon(IconNames.Happy)
    basic.pause(500)
    basic.showString("^")
})
```

--- feedback ---
Φοβερό! Όταν ο χρήστης γέρνει το micro:bit του προς τα αριστερά, μπορεί να επιλέξει τη διάθεσή του.
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
Αυτή είναι μια συνάρτηση για την απάντησή σου και δεν θα επιτρέψει στον χρήστη να επιλέξει τη διάθεσή του.
--- /feedback ---

- ( )

```microbit
basic.forever(function () {
    datalogger.log(datalogger.createCV("", 0))
})
```

--- feedback ---
Αυτό το μπλοκ κώδικα θα σε βοηθήσει να καταγράψεις δεδομένα από τις εισόδους του αισθητήρα στο micro:bit.
--- /feedback ---

- ( )

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.clearScreen()
})
```

--- feedback ---
Αυτό είναι ένα μπλοκ χειρονομίας που θα καθαρίσει την οθόνη του micro:bit, αλλά δεν θα αφήσει τον χρήστη να επιλέξει τη διάθεσή του.
--- /feedback ---

--- /choices ---

--- /question ---
