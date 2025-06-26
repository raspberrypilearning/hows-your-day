## Créer une réponse

Bien joué, tu as créé des humeurs parmi lesquelles ton utilisateur·trice peut choisir.
Tu vas maintenant utiliser un événement pour déclencher une réponse.

### Régler ton humeur

\--- collapse ---

---

## title: Pourquoi utiliser des événements ?

Les évènements sont une bonne option si tu souhaites que l'utilisateur·trice interagisse avec le programme.

Par exemple, dans le karaoké vérificateur d'humeur, les gestes étaient utilisés pour choisir parmi un ensemble d'humeurs, puis l'utilisateur·trice appuyait sur le Bouton A pour définir son choix.

\--- /collapse ---

\--- task ---

#### Utiliser les évènements

Ajoute le bloc d'évènement de ton choix dans ton espace de travail.

[[[microbit-buttons]]]

Par exemple, dans l'animateur d'humeur, le bloc `sur le logo appuyé`{:class='microbitinput'} est utilisé.

\--- /task ---

### Créer ta première réponse

Maintenant que tu as choisi un bloc d'évènement, tu as besoin de programmer une réponse à l'intérieur de celui-ci.

\--- task ---

Fais glisser un bloc `si`{:class='microbitlogic'} depuis le menu `Logique`{:class='microbitlogic'}.

Mets-le à l'intérieur de ton bloc d'évènement.

Dans cet exemple, le bloc `lorsque le bouton`{:class='microbitinput'} a été utilisé.

```microbit
input.onButtonPressed(Button.A, function () {
    if (true) {
    	
    }
})
```

\--- /task ---

\--- task ---

Ouvre le menu Logique{:class='microbitlogic'} et choisis le bloc `0 = 0`{:class='microbitlogic'}.

Place-le à l'intérieur de la partie `vrai`{:class='microbitlogic'} de l'énoncé `si`{:class='microbitlogic'}.

\--- /task ---

\--- task ---

Fais glisser ton bloc de variables `humeur`{:class='microbitvariables'} et place-le à l'intérieur du `0` à gauche du bloc `0 = 0`{:class='microbitlogic'}.

\--- /task ---

\--- task ---

Remplace le `0` à droite du bloc `0 = 0`{:class='microbitlogic'} par `1`.

Tes blocs de code pourraient ressembler à ceci :

```microbit
input.onButtonPressed(Button.AB, function () {
    if (mood == 1) {
    	
    }
})
```

\--- /task ---

\--- task ---

Ajoute un bloc de réponse à l'intérieur du bloc `si`{:class='microbitlogic'}.

Tu peux afficher une icône, une animation ou jouer de la musique.

[[[microbit-icons]]]
[[[microbit-animation]]]
[[[microbit-playing-sounds]]]

\--- /task ---

### Teste ton programme

\--- task ---

Lorsque le simulateur redémarre, utilise un geste pour choisir ton humeur.

Utilise ton événement pour déclencher ta réponse.

\--- /task ---
