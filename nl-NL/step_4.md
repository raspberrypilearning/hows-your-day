## Meer antwoorden maken

Voor elke stemming die je gebruiker heeft gekozen, kun je iets tonen of een activiteit geven.

\--- task ---

Voeg meer reacties toe aan je `wanneer knop wordt ingedrukt`{:class='microbitinput'} blok voor de andere antwoordopties.

Klik op de `+` knop onderaan je `als`{:class='microbitlogic'} blok om `anders als`{:class='microbitlogic'} blokken toe te voegen.

\[\[\[microbit-making-choices]]]

\--- /task ---

\--- task ---

Gebruik je micro:bit vaardigheden om meer antwoorden te maken.

Voeg ze toe in de `anders als`{:class='microbitlogic'} blokken.

Misschien herinner je deze dingen die je al gedaan hebt in de Verkennen projecten, die je misschien wilt gebruiken.

#### De LED's gebruiken

\[\[\[microbit-icons]]]

\[\[\[microbit-animation]]]

\[\[\[microbit-text]]]

\[\[\[microbit-plot-graph]]]

#### Geluid gebruiken

\[\[\[microbit-playing-sounds]]]

\[\[\[microbit-mic]]]

\[\[\[microbit-volume]]]

#### Overig

\[\[\[microbit-timer]]]

\[\[\[microbit-counting]]]

Kijk eens naar de projecten die je tijdens het pad al hebt gemaakt, om ideeën op te doen voor je antwoorden.

Hier is een voorbeeld van antwoorden die je kunt toevoegen:

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

### Functies gebruiken om je antwoorden te ordenen

Voor elk antwoord kun je een functie maken voor de activiteit die aan je gebruiker wordt getoond.

Hiermee wordt je code overzichtelijker, als je veel blokken hebt geplaatst in elk 'als'{:class='microbitlogic'} en 'anders als'{:class='microbitlogic'} blok.

Je kunt drie functies maken voor de drie antwoorden die je gebruiker te zien krijgt.

\--- task ---

\[\[\[microbit-function]]]

\--- /task ---

\--- task ---

Sleep je antwoordblokken naar je nieuwe functieblokken.

Hier is een voorbeeldcode van een functieblok:

```microbit
function goodDay () {
    basic.clearScreen()
    basic.showString("Sing!")
    basic.pause(100)
    music.play(music.stringPlayable("C C G G A A G - ", 120), music.PlaybackMode.LoopingInBackground)
}
```

\--- /task ---

Je moet je functie binnen je gebeurtenisblok aanroepen om deze te gebruiken.

\--- task ---

Vanuit de `Geavanceerd` sectie van de Toolbox sleep je `aanroep`{:class='microbitfunctions'} blokken van het `Functies`{:class='microbitfunctions'} menu.

Zorg ervoor dat je het juiste antwoord aanroep blok gebruikt.

Plaats deze blokken in de `als`{:class='microbitlogic'} en `anders als`{:class='microbitlogic'} blokken in je gebeurtenis.

\--- /task ---

### Je programma opnieuw instellen

Zodra een gebruiker zijn stemming heeft ingesteld en een antwoord heeft gegeven, kun je hem toestaan het programma te resetten en opnieuw te beginnen.

\--- task ---

Vanuit het `Invoer`{:class='microbitinput'} menu sleep je een gebeurtenis blok dat je nog niet hebt gebruikt in je project.

Plaats het in je bewerkingspaneel.

\--- /task ---

\--- task ---

Vanuit het `Muziek`{:class='microbitmusic'} menu sleep je een `stop alle geluiden`{:class='microbitmusic'} blok.

Plaats het in je gebeurtenis blok.

Het blok `bij logo ingedrukt`{:class='microbitinput'} is gebruikt in dit voorbeeld.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
})
```

\--- /task ---

\--- task ---

Dupliceer je startscherm blokken of de startscherm functie.

Plaats het onder het blok `stop alle geluiden`{:class='microbitmusic'}.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
    startupScreen()
})
```

\--- /task ---

### Test je programma

\--- task ---

Wanneer de simulator opnieuw opstart, gebruik dan een gebaar om je stemming te kiezen.

Gebruik je gebeurtenis om je antwoord te triggeren.

Gebruik je andere gebeurtenis blok om het programma opnieuw in te stellen.

\--- /task ---

\[\[\[download-to-microbit]]]

Nu is het tijd om te kijken wat je hebt geleerd!
