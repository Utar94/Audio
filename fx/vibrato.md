# Vibrato

## Définition

Le Vibrato est un effet audio (FX) de modulation qui consiste à faire osciller périodiquement la hauteur (Pitch) d’un son autour de sa note originale. Il produit une légère variation de tonalité qui donne une impression de mouvement et d’expressivité, sans modifier directement le volume. Le Vibrato peut être généré naturellement par un musicien ou artificiellement par un synthétiseur ou un plugin audio.

## Utilité

Le Vibrato permet d’ajouter de l’expressivité, de la chaleur et du mouvement à un son, en le rendant plus vivant et moins statique. Il est particulièrement utilisé sur les voix, les instruments à cordes, les guitares et les synthétiseurs Lead pour imiter les variations naturelles d’un instrumentiste. Selon son intensité et sa vitesse, il peut produire une oscillation subtile et musicale ou un effet beaucoup plus prononcé, instable et psychédélique.

## Fonctionnement

Le Vibrato fonctionne en faisant varier automatiquement la hauteur du son grâce à un oscillateur basse fréquence appelé LFO (Low Frequency Oscillator). Ses principaux paramètres sont le Rate, qui détermine la vitesse des oscillations en Hertz, le Depth, qui contrôle l’amplitude des variations de hauteur, généralement exprimée en cents ou en demi-tons, et parfois le Delay, qui définit le temps avant l’apparition du Vibrato. Contrairement au Tremolo, qui fait varier le volume, le Vibrato agit exclusivement sur la hauteur des notes.

## VST3: MVibrato (MeldaProduction)

MVibrato est un plugin audio de MeldaProduction qui permet de créer un effet de Vibrato en faisant osciller automatiquement la hauteur des notes, avec la possibilité d’ajouter une modulation de volume de type Tremolo.

| Paramètre                 | Valeur                 |
| ------------------------- | ---------------------- |
| Depth                     | 🛞**Modulation Wheel** |
| Rate                      | ⚙️**Knob**             |
| Width                     | 0°                     |
| Tremolo                   | 0%                     |
| Tremolo Phase             | 0°                     |
| Invert Tremolo Phase      | Désactivé              |
| Simulate Realistic Shapes | Désactivé              |
| LFO Override              | Auto                   |

### Depth

> Contrôle la profondeur du Vibrato, c’est-à-dire l’amplitude des variations de hauteur appliquées au son original.

- Augmenter : Accentue les variations de hauteur, créant un Vibrato plus expressif, voire instable ou psychédélique.
- Diminuer : Réduit les variations de hauteur, produisant un Vibrato plus subtil. À 0 %, le Vibrato disparaît.
- Cette plage permet de passer d’un son sans Vibrato à une modulation bien perceptible, sans atteindre les réglages les plus extrêmes. Une valeur initiale de 10 % constitue un point de départ prudent pour préserver la justesse des notes.
- Pour un Vibrato naturel, les profondeurs se situent souvent autour de quelques dizaines de cents, selon l’instrument. Dans MVibrato, le Depth est exprimé en pourcentage et ne correspond pas directement à une valeur universelle en cents. La plage 0–30 % est donc une proposition à tester à l’oreille.

### Rate (Hz)

> Contrôle la vitesse des oscillations du Vibrato, exprimée en Hertz (cycles par seconde).

- Augmenter : Accélère les variations de hauteur, produisant un Vibrato plus nerveux et intense.
- Diminuer : Ralentit les oscillations, créant un mouvement plus doux, lent et progressif.
- Une fréquence de 5 Hz correspond à cinq oscillations par seconde, ce qui donne un Vibrato expressif et relativement naturel. La plage de 3 à 8 Hz permet de passer d’un mouvement lent à un Vibrato rapide sans atteindre les vitesses extrêmes du plugin.
- Les Vibratos naturels des voix et de nombreux instruments se situent fréquemment autour de 4–7 Hz, avec des variations selon le style et l’instrument. La valeur de 10,15 Hz affichée dans ta capture est relativement rapide pour un Vibrato naturel.

### Width

> Contrôle la différence de phase entre les modulations appliquées aux canaux gauche et droit, permettant de créer un mouvement stéréo.

- Augmenter : Modifie le décalage entre les oscillations des canaux, pouvant créer une impression de mouvement plus large.
- Diminuer : Rapproche les phases des modulations. À 0°, les canaux oscillent ensemble.
- La largeur n’augmente pas continuellement avec la valeur : un décalage de 360° ramène les oscillations en phase.
- Une valeur de 0° applique un mouvement cohérent aux deux canaux et conserve une hauteur perçue relativement stable dans l’image stéréo. C’est préférable pour un Lead mélodique.
- Les valeurs de 0° et 180° sont des points de départ fréquents pour les modulations stéréo. Le choix dépend du résultat recherché; un Vibrato expressif traditionnel ne nécessite pas de décalage entre les canaux.

### Tremolo

> Contrôle l’intensité d’un effet de Tremolo supplémentaire, qui fait osciller le volume du son plutôt que sa hauteur.

- Augmenter : Accentue les variations périodiques du volume, produisant un effet pulsant ou tremblant.
- Diminuer : Réduit les oscillations du volume. À 0 %, le Tremolo est désactivé.
- Je recommande de désactiver le Tremolo afin que MVibrato serve exclusivement à modifier la hauteur des notes. Cela permet de conserver une distinction claire entre les deux effets.
- Le Vibrato et le Tremolo sont généralement considérés comme deux types de modulation distincts. Il n’existe pas de pourcentage standard pour les mélanger, et un Tremolo à 0 % convient lorsque seul le Vibrato est recherché.

### Tremolo Phase

> Définit le décalage de phase entre les oscillations du Tremolo et celles du Vibrato.

- Augmenter : Décale progressivement le mouvement du Tremolo par rapport au Vibrato, modifiant leur interaction.
- Diminuer : Rapproche les mouvements des deux modulations. À 0°, elles utilisent la même référence de phase.
- Puisque le Tremolo est désactivé, ce paramètre n’aura aucun effet audible. Il peut donc rester à sa valeur par défaut.
- Aucun réglage universel. Les décalages de phase sont principalement utilisés lorsque plusieurs modulations sont combinées pour créer des textures rythmiques ou expérimentales.

### Invert Tremolo Phase

> Inverse la forme de modulation du Tremolo, modifiant les moments où le volume augmente et diminue.

- Activé : Inverse le mouvement du Tremolo, transformant ses augmentations de volume en diminutions, et inversement.
- Désactivé : Conserve la forme de modulation originale.
- Cette option n’est pas utile puisque nous désactivons le Tremolo. Elle peut rester à sa valeur par défaut.
- Aucun standard particulier. L’inversion est surtout employée dans les effets combinant plusieurs modulations.

### Simulate Realistic Shapes

> Active un traitement supplémentaire qui cherche à reproduire plus fidèlement le comportement d’un Vibrato naturel.

- Activé : Modifie le traitement pour tenter de reproduire certaines caractéristiques d’un Vibrato généré directement par un instrument.
- Désactivé : Conserve le traitement standard du plugin.
- Je recommande de commencer avec le traitement standard, plus simple à évaluer. Tu pourras ensuite comparer les deux modes et conserver celui qui convient le mieux à ta banque de sons.
- Cette option est propre à MVibrato et ne possède pas de standard universel. Les traitements destinés à reproduire un Vibrato naturel sont courants, mais leur fonctionnement varie selon les plugins.

### LFO Override

> Permet de remplacer l’oscillation automatique du LFO par une position de modulation contrôlée directement.

- Lorsque l’Override est actif, modifier sa valeur déplace manuellement la position de modulation, plutôt que de laisser le LFO osciller automatiquement.
- Le mode Auto conserve l’oscillation automatique nécessaire au Vibrato. Nous souhaitons contrôler sa profondeur et sa vitesse, pas déplacer manuellement chaque oscillation.
- Le fonctionnement automatique par LFO est le plus courant pour le Vibrato. Le contrôle manuel est principalement utilisé pour des effets expérimentaux ou des automatisations particulières.

## Résumé des affectations MIDI

## Pourquoi Depth et Rate ?

Depth (knob AKAI + fader Arturia) permet de faire apparaître progressivement le Vibrato, jusqu’à obtenir une variation de hauteur très prononcée. Contrairement à un contrôle Wet traditionnel, il modifie directement la profondeur de l’oscillation.

Rate (knob Arturia) permet de modifier la vitesse du Vibrato indépendamment de son intensité. Un mouvement lent pourra produire un effet doux et expressif, tandis qu’un mouvement rapide créera un son plus nerveux ou instable.

Cette configuration respecte aussi notre nouvelle convention :

- Faders Arturia : quantité d’effet.
- Knobs Arturia : caractère de l’effet.
- Knobs AKAI : quantité d’effet, puisque l’AKAI ne possède pas de faders.

Ma recommandation : commence avec un Depth maximum de 30 % et un Rate fixe de 5 Hz sur l’AKAI. Comme la profondeur de MVibrato n’est pas exprimée en cents, il faudra tester ce maximum sur tes sons de Lead avant de le conserver définitivement.
