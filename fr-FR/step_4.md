## Créer plusieurs réponses

Pour toute humeur que ton utilisateur·trice a choisie, tu peux lui montrer quelque chose ou lui donner une activité à faire.

\--- task ---

Ajoute d'autres réponses à ton bloc `lorsque le bouton`{:class='microbitinput'} pour les autres options de réponse.

Clique sur le bouton `+` en bas de ton bloc `si`{:class='microbitlogic'} pour ajouter des blocs `sinon`{:class='microbitlogic'}.

[[[microbit-making-choices]]]

\--- /task ---

\--- task ---

Utilise tes compétences micro:bit pour créer plus de réponses.

Place-les à l'intérieur des blocs `sinon`{:class='microbitlogic'}.

Voici quelques rappels de ce que tu as déjà fait dans les projets Explorer et que tu pourrais utiliser.

#### Utiliser les LED

[[[microbit-icons]]]

[[[microbit-animation]]]

[[[microbit-text]]]

[[[microbit-plot-graph]]]

#### Utiliser les sons

[[[microbit-playing-sounds]]]

[[[microbit-mic]]]

[[[microbit-volume]]]

#### Autre

[[[microbit-timer]]]

[[[microbit-counting]]]

Jette un œil aux projets que tu as réalisés auparavant pour t'en inspirer dans tes réponses.

Voici un exemple de réponses que tu pourrais ajouter :

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

### Utiliser des fonctions pour organiser tes réponses

Pour chaque réponse, tu peux créer une fonction pour l'opération qui sera affichée à ton utilisateur·trice.

Cela mettra de l'ordre dans ton code si tu as beaucoup de blocs à l'intérieur de chaque bloc `si`{:class='microbitlogic'} et `sinon`{:class='microbitlogic'}.

Tu peux créer trois fonctions pour les trois réponses affichées à ton utilisateur·trice.

\--- task ---

[[[microbit-function]]]

\--- /task ---

\--- task ---

Fais glisser tes blocs de réponse dans tes nouveaux blocs de fonctions.

Voici un exemple de code d'un bloc de fonction :

```microbit
function goodDay () {
    basic.clearScreen()
    basic.showString("Sing!")
    basic.pause(100)
    music.play(music.stringPlayable("C C G G A A G - ", 120), music.PlaybackMode.LoopingInBackground)
}
```

\--- /task ---

Tu devras nommer ta fonction à l'intérieur de ton bloc événement pour l'utiliser.

\--- task ---

Depuis la section `Avancé` de la Boîte à outils, fais glisser tes blocs `appel`{:class='microbitfunctions'} depuis le menu `Fonctions`{:class='microbitfunctions'}.

Assure-toi d'utiliser le bon bloc d'appel de réponse.

Place ces blocs à l'intérieur des blocs `si`{:class='microbitlogic'} et `sinon`{:class='microbitlogic'} dans ton événement.

\--- /task ---

### Réinitialiser ton programme

Une fois qu'un utilisateur a défini son humeur et complété une réponse, tu peux lui permettre de réinitialiser le programme et de recommencer.

\--- task ---

À partir du menu `Entrée`{:class='microbitinput'}, fais glisser un bloc d'événements que tu n'as pas encore utilisé dans ton projet.

Place-le dans ton espace de travail.

\--- /task ---

\--- task ---

Depuis le menu `Musique`{:class="microbitmusic"}, fais glisser le bloc `arrêter tous les sons`{:class="microbitmusic"}.

Mets-le à l'intérieur de ton bloc évènement.

Le bloc `sur le logo appuyé`{:class='microbitloops'} a été utilisé dans cet exemple.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
})
```

\--- /task ---

\--- task ---

Duplique tes blocs d'écran de démarrage ou ta fonction d'écran de démarrage.

Place la duplication sous le bloc `arrêter tous les sons`{:class="microbitmusic"}.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    music.stopAllSounds()
    startupScreen()
})
```

\--- /task ---

### Teste ton programme

\--- task ---

Lorsque le simulateur redémarre, utilise un geste pour choisir ton humeur.

Utilise ton événement pour déclencher ta réponse.

Utilise ton autre bloc événement pour réinitialiser le programme.

\--- /task ---

[[[download-to-microbit]]]

Ensuite, il est temps de vérifier ce que tu as appris !
