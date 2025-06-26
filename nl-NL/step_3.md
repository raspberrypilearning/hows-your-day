## Maak een antwoord

Goed gedaan, je hebt de stemmingen gemaakt waaruit je gebruiker kan kiezen.
Je gaat nu een gebeurtenis gebruiken om een antwoord te vragen.

### Stel je stemming in

--- collapse ---

---
title: Waarom gebeurtenissen gebruiken?
---

Gebeurtenissen zijn een goede keuze als je wilt dat je gebruiker interactie heeft met het programma.

Bijvoorbeeld in de karaoke stemmingschecker werden gebaren gebruikt om te kiezen uit verschillende stemmingen, en vervolgens drukte de gebruiker op knop A om een keuze in te stellen.

--- /collapse ---

--- task ---

### Het gebruik van gebeurtenissen

Kies de blokken van de gebeurtenissen en voeg ze toe aan je bewerkingspaneel.

[[[microbit-buttons]]]
Bijvoorbeeld, in de stemmingsanimator wordt het blok `bij logo ingedrukt`{:class='microbitinput'} gebruikt.

--- /task ---

### Maak je eerste antwoord

Nu je een gebeurtenisblok hebt gekozen, ga je een antwoord erin programmeren.

--- task ---

Sleep een `als`{:class='microbitlogic'} blok uit het `Logisch`{:class='microbitlogic'} menu.

Plaats het in je gebeurtenis blok.

In dit voorbeeld is het `wanneer knop wordt ingedrukt`{:class='microbitinput'} blok gebruikt.

```microbit
input.onButtonPressed(Button.A, function () {
    if (true) {
    	
    }
})
```
--- /task ---

--- task ---

Open het `Logisch`{:class='microbitlogic'} menu en selecteer het `0 = 0`{:class='microbitlogic'} blok.

Plaats het in het `waar`{:class='microbitlogic'} deel van de `als`{:class='microbitlogic'} instructie.

--- /task ---

--- task ---

Sleep je `stemming`{:class='microbitvariables'} variabele blok en plaats het in het `0` blok aan de linkerkant van het `0 = 0`{:class='microbitlogic'} blok.

--- /task ---

--- task ---

Verander het `0` blok aan de rechterkant`0 = 0`{:class='microbitlogic'} naar `1`.

Je code blokken zouden er als volgt uit moeten zien:

```microbit
input.onButtonPressed(Button.AB, function () {
    if (stemming == 1) {
    	
    }
})
```

--- /task ---

--- task ---

Voeg een antwoordblok toe binnen het blok `als`{:class='microbitlogic'}.

Je kunt een pictogram of een animatie weergeven of wat muziek afspelen.

[[[microbit-icons]]]
[[[microbit-animation]]]
[[[microbit-playing-sounds]]]

--- /task ---

### Test je programma

--- task ---

Wanneer de simulator opnieuw opstart, gebruik dan een gebaar om je stemming te kiezen.

Gebruik je gebeurtenis om je antwoord te triggeren.

--- /task ---
