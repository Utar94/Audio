# Tremolo

## Définition

Le Tremolo est un effet audio (FX) de modulation qui consiste à faire osciller périodiquement le volume d’un son, créant une impression de pulsation ou de vibration rythmique. Contrairement au Vibrato, qui modifie la hauteur (Pitch) des notes, le Tremolo agit uniquement sur leur intensité sonore, sans modifier leur tonalité.

## Utilité

Le Tremolo permet d’ajouter du mouvement, du rythme et de l’expressivité à un son en faisant varier automatiquement son volume. Il est particulièrement utilisé sur les guitares, les pianos électriques, les synthétiseurs et les Pads pour créer des ambiances douces et ondulantes ou des pulsations rapides et saccadées. Selon son intensité et sa vitesse, il peut produire un effet subtil et naturel ou un effet rythmique très prononcé, proche d’une succession de coupures sonores.

## Fonctionnement

Le Tremolo fonctionne en faisant varier automatiquement l’amplitude du signal audio grâce à un oscillateur basse fréquence appelé LFO (Low Frequency Oscillator). Ses principaux paramètres sont le Rate, qui détermine la vitesse des oscillations en Hertz ou en divisions musicales synchronisées au tempo, le Depth, qui contrôle l’intensité des variations de volume, et le Shape, qui définit la forme des oscillations. Une onde sinusoïdale produit des variations douces et progressives, tandis qu’une onde carrée crée des alternances brusques entre les niveaux sonores, pouvant produire un effet de coupure rythmique (chopping).

## VST3: MTremolo (MeldaProduction)

MTremolo est un plugin audio de MeldaProduction qui permet de faire osciller automatiquement le volume d’un son, créant des pulsations rythmiques dont la vitesse, la profondeur et la forme peuvent être personnalisées.

| Paramètre            | Valeur    |
| -------------------- | --------- |
| Depth                | ❓        |
| Rate                 | ❓        |
| Width                | 0°        |
| LFO Override         | Auto      |
| Invert Tremolo Phase | Désactivé |
| Sync                 | Désactivé |
| Shape (LFO)          | Sine      |
| Custom               | 0 %       |
| Step                 | 0 %       |
| Smooth               | 0 %       |
| Normal / Harmonics   | Normal    |

### Depth

> Contrôle la profondeur du Tremolo, c’est-à-dire l’intensité des variations de volume.

- Augmenter : Accentue les variations de volume, créant des pulsations plus prononcées pouvant aller jusqu’à des coupures rythmiques.
- Diminuer : Réduit les variations, produisant un Tremolo plus subtil. À 0 %, l’effet est inaudible.
- Cette plage permet de passer d’un son naturel à des pulsations très marquées, sans atteindre systématiquement les coupures les plus extrêmes. Une valeur initiale de 0 % garantit que l’effet n’est appliqué que lorsque tu le souhaites.
- Une profondeur approximative de 10–40 % est un point de départ courant pour un Tremolo subtil ou modéré. Des valeurs de 50–100 % servent à créer des pulsations très prononcées et des effets de découpage rythmique. Le résultat exact dépend de la façon dont chaque plugin définit sa profondeur.

### Rate (Hz)

> Contrôle la vitesse des oscillations du volume, exprimée en Hertz (cycles par seconde).

- Augmenter : Accélère les pulsations, créant un Tremolo plus nerveux et rythmé.
- Diminuer : Ralentit les pulsations, produisant un mouvement plus doux et progressif.
- Une valeur de 4,5 Hz produit des pulsations rapides, mais encore distinctes. La plage 0,5–8 Hz permet d’explorer des mouvements très lents jusqu’à des oscillations rapides, sans atteindre la limite de 20 Hz offerte par MTremolo.
- Les Tremolos classiques utilisent fréquemment des vitesses d’environ 2–8 Hz. Les valeurs inférieures à 2 Hz donnent des pulsations lentes et atmosphériques, tandis que les valeurs plus élevées produisent des textures plus agitées.

### Width

> Contrôle la différence de phase entre les modulations de volume appliquées aux canaux gauche et droit, permettant de créer un mouvement stéréo.

- Augmenter vers 180° : Accentue le décalage entre les pulsations gauche et droite, pouvant créer une impression de mouvement alterné entre les haut-parleurs.
- Diminuer vers 0° : Synchronise progressivement les pulsations entre les deux canaux.
- À 360° : Les modulations se retrouvent en phase.
- Une valeur de 0° conserve les pulsations synchronisées dans les deux canaux, ce qui permet de faire varier le volume sans déplacer artificiellement la position stéréo de l’instrument.
- Les décalages de 0° et 180° sont des points de départ fréquents. Le premier produit un Tremolo classique, tandis que le second permet d’obtenir un mouvement stéréo plus prononcé.

### LFO Override

> Permet de remplacer les oscillations automatiques du LFO par une position de modulation contrôlée manuellement ou par automatisation.

- Augmenter : Déplace la modulation vers une autre position de sa courbe, modifiant directement le niveau sonore.
- Diminuer : Déplace la modulation dans le sens inverse.
- Lorsque l’Override est actif, le LFO ne produit plus son mouvement périodique habituel.
- Le mode Auto conserve le Tremolo automatique. Nous souhaitons contrôler sa vitesse et son intensité, sans devoir déplacer manuellement les oscillations.
- Le fonctionnement automatique par LFO est habituel pour les Tremolos. Le contrôle manuel est principalement utilisé pour des effets créatifs et des automatisations particulières.

### Invert Tremolo Phase

> Inverse la forme de modulation du Tremolo, en échangeant les moments où le volume augmente et diminue.

- Activé : Les augmentations de volume deviennent des diminutions, et inversement.
- Désactivé : Conserve la forme de modulation originale.
- L’inversion n’est pas nécessaire pour un Tremolo classique. Avec une seule modulation sinusoïdale, elle revient principalement à décaler le cycle d’une demi-période.
- Aucun standard particulier. L’inversion peut être intéressante pour synchroniser plusieurs instruments ayant des pulsations complémentaires.
