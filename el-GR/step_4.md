## Δημιουργία περισσότερων απαντήσεων

Για οποιαδήποτε διάθεση έχει επιλέξει ο χρήστης, μπορείς να τους δείξεις κάτι ή να τους δώσεις μια δραστηριότητα να κάνουν.

\--- task ---

Πρόσθεσε περισσότερες απαντήσεις στο μπλοκ "όταν πιεστεί το πλήκτρο"{:class='microbitinput'} για τις άλλες επιλογές απάντησης.

Κάνε κλικ στο κουμπί `+` στο κάτω μέρος του μπλοκ `εάν`{:class='microbitlogic'} για να προσθέσεις τα μπλοκ `αλλιώς εάν`{:class='microbitlogic'}.

[[[microbit-making-choices]]]

\--- /task ---

\--- task ---

Χρησιμοποίησε τις δυνατότητες του micro:bit για να δημιουργήσεις περισσότερες απαντήσεις.

Πρόσθεσέ τα μέσα στο μπλοκ εάν{:class='microbitlogic'}.

Ακολουθούν ορισμένες υπενθυμίσεις για πράγματα που έχεις ήδη κάνει στα έργα Εξερεύνησης που ίσως θέλεις να χρησιμοποιήσεις.

#### Χρήση των LED

[[[microbit-icons]]]

[[[microbit-animation]]]

[[[microbit-text]]]

[[[microbit-plot-graph]]]

#### Χρήση ήχων

[[[microbit-playing-sounds]]]

[[[microbit-mic]]]

[[[microbit-volume]]]

#### Άλλο

[[[microbit-timer]]]

[[[microbit-counting]]]

Ρίξε μια ματιά στα έργα που έχεις κάνει σε όλη τη διαδρομή για να πάρεις έμπνευση για τις απαντήσεις σου.

Εδώ είναι ένα παράδειγμα των απαντήσεων που μπορείς να προσθέσεις:

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

\--- /task ---

### Χρήση συναρτήσεων για να οργανώσεις τις απαντήσεις σου

Για κάθε απάντηση, μπορείς να δημιουργήσεις μια συνάρτηση για τη δραστηριότητα που θα εμφανίζεται στον χρήστη σου.

Αυτό θα τακτοποιήσει τον κώδικά σου αν έχεις πολλά μπλοκ μέσα σε κάθε μπλοκ `εάν`{:class='microbitlogic'} και `αλλιώς εάν`{:class='microbitlogic'}.

Θα μπορούσες να δημιουργήσεις τρεις συναρτήσεις για τις τρεις απαντήσεις που εμφανίζονται στον χρήστη σου.

\--- task ---

[[[microbit-function]]]

\--- /task ---

\--- task ---

Σύρε τα μπλοκ απάντησης στα μπλοκ συναρτήσεων που δημιούργησες πρόσφατα.

Ακολουθεί ένα παράδειγμα κώδικα από ένα μπλοκ συνάρτησης:

```microbit
function goodDay () {
    basic.clearScreen()
    basic.showString("Sing!")
    basic.pause(100)
    music.play(music.stringPlayable("C C G G A A G - ", 120), music.PlaybackMode.LoopingInBackground)
}
```

\--- /task ---

Θα χρειαστεί να καλέσεις τη συνάρτησή σου μέσα στο μπλοκ συμβάντων για να τηνχρησιμοποιήσεις.

\--- task ---

Από την ενότητα "Για προχωρημένους" της Εργαλειοθήκης, σύρε τα μπλοκ "κλήση"{:class='microbitfunctions'} από το μενού "Συναρτήσεις"{:class='microbitfunctions'}.

Βεβαιώσου ότι χρησιμοποιείς το σωστό μπλοκ κλήσης για την απάντηση.

Τοποθέτησε αυτά τα μπλοκ μέσα στα μπλοκ `εάν`{:class='microbitlogic'} και `αλλιώς εάν`{:class='microbitlogic'} στο συμβάν σου.

\--- /task ---

### Επανεκκίνηση του προγράμματός σου

Μόλις ένας χρήστης ορίσει τη διάθεσή του και ολοκληρωθεί μια απάντηση, μπορείς να τους επιτρέψεις να επανεκκινήσει το πρόγραμμα και να ξεκινήσει ξανά.

\--- task ---

Από το μενού "Είσοδος"{:class='microbitinput'}, σύρε ένα μπλοκ συμβάντων που δεν έχεις χρησιμοποιήσει ακόμη στο έργο σου.

Τοποθέτησέ το στον χώρο εργασίας σου.

\--- /task ---

\--- task ---

Από το μενού `Music`{:class='microbitmusic'} σύρε ένα μπλοκ `stop all sounds`{:class='microbitmusic'}.

Τοποθέτησέ το μέσα στο μπλοκ συμβάντος.

Το μπλοκ `on logo pressed`{:class='microbitinput'} έχει χρησιμοποιηθεί σε αυτό το παράδειγμα.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
})
```

\--- /task ---

\--- task ---

Αντίγραψε τα μπλοκ της αρχικής οθόνης ή τη λειτουργία της αρχικής οθόνης.

Τοποθέτησέ το κάτω από το μπλοκ `stop all sounds`{:class='microbitmusic'}.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
    startupScreen()
})
```

\--- /task ---

### Δοκίμασε το έργο σου

\--- task ---

Όταν ο προσομοιωτής επανεκκινηθεί, χρησιμοποίησε μια χειρονομία για να επιλέξεις τη διάθεσή σου.

Χρησιμοποίησε το συμβάν για να ενεργοποιήσεις την απάντησή σου.

Χρησιμοποίησε το άλλο μπλοκ συμβάντων για να επανεκκινήσεις το πρόγραμμα.

\--- /task ---

[[[download-to-microbit]]]

Στη συνέχεια, ήρθε η ώρα να ελέγξεις τι έχεις μάθει!
