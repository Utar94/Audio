# Phaser

## Définition

Le Phaser est un effet audio qui modifie certaines fréquences d’un son en créant un mouvement de balayage caractéristique, souvent décrit comme un effet tourbillonnant, liquide ou psychédélique. Il donne l’impression que le son se déplace ou change continuellement de texture, sans nécessairement modifier la hauteur des notes jouées.

## Utilité

Le Phaser permet d’ajouter du mouvement, de la profondeur et du caractère à un son. Il est particulièrement utilisé sur les synthétiseurs, les guitares, les pianos électriques et les Pads pour créer des textures évolutives et des ambiances psychédéliques. Il peut produire un mouvement subtil qui enrichit un instrument ou un balayage très prononcé qui transforme radicalement sa sonorité.

## Fonctionnement

Le Phaser fonctionne en décalant la phase de certaines fréquences du signal audio, puis en mélangeant ce signal modifié avec le son original. Ce mélange provoque des annulations partielles à certaines fréquences, créant des creux dans le spectre sonore qui se déplacent grâce à une modulation périodique appelée LFO (Low Frequency Oscillator). Plusieurs paramètres permettent de contrôler cet effet, notamment le Rate, qui détermine la vitesse du balayage, le Depth, qui contrôle son amplitude, le Feedback, qui accentue les résonances, et le Dry/Wet, qui ajuste le mélange entre le son original et le son traité.

## VST3: MPhaser (MeldaProduction)

MPhaser est un plugin audio de MeldaProduction qui crée un effet de Phaser en faisant varier le déphasage de certaines fréquences, produisant un balayage sonore caractéristique, parfois tourbillonnant, liquide ou psychédélique.

| Paramètre     | Valeur               |
| ------------- | -------------------- |
| Dry/Wet       | ⚙️**Knob**           |
| Min Frequency | 400 Hz               |
| Max Frequency | 2500 Hz              |
| Rate          | 🎚️**Fader** (0.5 Hz) |
| Feedback      | -12 dB               |
| Mode          | 4                    |
| Mode          | 180°                 |
| Saturation    | 0%                   |

### Dry/Wet

> Contrôle le mélange entre le son original (Dry) et le son traité par le Phaser (Wet).

- Augmenter le Dry/Wet rend le Phaser plus présent et accentue ses balayages. Le diminuer réduit l’intensité de l’effet jusqu’à retrouver uniquement le son original à 0 %.
- Cette plage permet de passer d’un son complètement sec à un Phaser prononcé, sans atteindre les mélanges extrêmes. Une valeur de 35 % offre un mouvement audible tout en conservant le caractère original de l’instrument.
- Les mélanges de 20–50 % sont de bons points de départ pour les Phasers classiques. Un mélange proche de 50 % peut produire des annulations de fréquences particulièrement marquées, tandis qu’à 100 %, le Phaser ne mélange plus le signal traité avec le signal original de la même manière.

### Min Frequency

> Définit la fréquence minimale atteinte par le balayage du Phaser.

- Augmenter la valeur déplace la limite inférieure du balayage vers les fréquences plus aiguës. La diminuer permet au mouvement d’atteindre des fréquences plus graves, donnant potentiellement un caractère plus profond.
- Une fréquence minimale de 400 Hz permet de concentrer le balayage sur les fréquences moyennes sans trop affecter les graves, ce qui convient bien à tes instruments mélodiques.
- Il n’existe pas de standard universel, mais des valeurs de départ autour de 200–600 Hz sont raisonnables pour explorer un Phaser destiné aux synthétiseurs.

### Max Frequency

> Définit la fréquence maximale atteinte par le balayage du Phaser.

- Augmenter la valeur permet au balayage d’atteindre davantage de fréquences aiguës, donnant un effet plus brillant. La diminuer concentre le mouvement dans une région plus grave du spectre sonore.
- Une fréquence maximale de 2 500 Hz permet de balayer une bonne partie des fréquences moyennes et aiguës, sans rendre le Phaser excessivement brillant.
- Les fréquences maximales autour de 1 500–5 000 Hz constituent des points de départ courants pour expérimenter les balayages de Phaser. La plage exacte dépend beaucoup du caractère recherché.

### Rate (Hz)

> Contrôle la vitesse du LFO (Low Frequency Oscillator), qui fait varier continuellement le balayage du Phaser.

- Augmenter le Rate accélère les mouvements du Phaser, produisant un effet plus agité, parfois proche d’une modulation rapide et tourbillonnante. Le diminuer ralentit le balayage, créant un mouvement plus doux, progressif et atmosphérique.
- Une valeur de 0,5 Hz correspond à un cycle complet toutes les deux secondes, donnant un mouvement relativement lent mais perceptible. La plage du fader permet d’explorer des mouvements subtils jusqu’à des balayages nettement plus rapides.
- Les Phasers classiques utilisent fréquemment des modulations lentes, approximativement entre 0,1 et 2 Hz. Des valeurs supérieures sont possibles pour des effets plus expérimentaux.

### Feedback

> Contrôle la quantité de signal traité qui est réinjectée dans le Phaser, afin d’accentuer ses résonances et son caractère sonore.

- Augmenter le Feedback vers 0 dB renforce les résonances et rend le balayage plus intense, parfois métallique ou sifflant. Le diminuer produit un Phaser plus doux, avec des creux et des résonances moins marqués.
- Une valeur de -12 dB apporte suffisamment de résonance pour rendre le balayage audible, sans produire un effet trop agressif. Comme tu disposes déjà d’autres effets expérimentaux, je préfère conserver un Feedback modéré.
- Les Phasers utilisent souvent un Feedback léger à modéré. Dans MPhaser, environ -18 à -6 dB constitue une plage d’exploration raisonnable, sachant que les valeurs proches de 0 dB peuvent produire des résonances beaucoup plus prononcées.

### Mode

> Détermine le nombre d’étages de déphasage utilisés par le plugin, ce qui modifie le nombre et la répartition des creux créés dans le spectre sonore.

- Augmenter le Mode complexifie le déphasage et peut créer une texture plus riche et plus particulière. Le diminuer produit généralement un Phaser plus simple, avec moins de variations dans le spectre.
- Une valeur de 4 correspond à un Phaser relativement classique. Elle produit un balayage distinctif sans introduire la complexité des configurations comportant de nombreux étages.
- Les Phasers traditionnels utilisent couramment 4, 6, 8 ou 12 étages selon le modèle. MPhaser permet d’aller jusqu’à 100, mais ces valeurs élevées relèvent davantage de la création sonore expérimentale.

### Width

> Contrôle la différence de phase entre les modulations appliquées aux canaux gauche et droit, créant une sensation de mouvement stéréo.

- À 0°, les deux canaux effectuent leur balayage ensemble. Vers 180°, leurs modulations sont opposées, créant un mouvement stéréo plus contrasté. À 360°, elles se retrouvent de nouveau synchronisées; augmenter le paramètre ne signifie donc pas toujours élargir davantage le son.
- Une différence de 180° permet d’obtenir un mouvement stéréo intéressant, particulièrement sur les Keys et les Pads. Le son paraît plus animé et enveloppant, sans nécessiter de modulation MIDI supplémentaire.
- Les décalages de 0° et 180° sont des points de départ classiques. Les réglages intermédiaires permettent d’obtenir des mouvements moins symétriques. Le résultat doit aussi être vérifié en mono pour éviter les problèmes d’annulation.

### Saturation

> Ajoute une saturation au signal traité par le Phaser, introduisant de nouvelles harmoniques et modifiant son caractère.

- Augmenter la Saturation rend le son plus riche, coloré et potentiellement agressif. La diminuer conserve un Phaser plus propre et transparent.
- Je suggère de désactiver la saturation pour conserver le Phaser comme un effet de modulation pur. Tu disposes déjà d’un effet de Distortion sur ton AKAI, ce qui permet de contrôler séparément ces deux transformations sonores.
- Une saturation légère est parfois utilisée pour reproduire le caractère des Phasers analogiques. Il n’existe toutefois pas de pourcentage standard, puisque chaque plugin utilise ses propres algorithmes.
