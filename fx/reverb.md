# Reverb

## Définition

La réverbération (Reverb) est un effet audio qui reproduit la manière dont un son résonne dans un espace. Lorsqu’un son est produit dans une pièce, une partie arrive directement à nos oreilles, tandis qu’une autre rebondit sur les murs, le plafond et les objets avant de nous parvenir. Ces nombreuses réflexions créent une résonance qui persiste brièvement après le son original.

## Utilité

La Reverb permet de donner de l’espace, de la profondeur et de l’ambiance à un son. Elle peut donner l’impression qu’un instrument est joué dans une petite pièce, une grande salle de concert ou une immense cathédrale. Elle aide aussi à rendre un son plus naturel, plus enveloppant ou plus atmosphérique. En production musicale, elle est souvent utilisée pour éviter que les instruments paraissent trop secs ou artificiels.

## Fonctionnement

La Reverb fonctionne en générant une multitude de réflexions du son original, avec de légers décalages dans le temps. Ces réflexions se mélangent et diminuent progressivement en intensité jusqu’à disparaître. Plusieurs paramètres permettent de modifier cet effet, notamment le Decay, qui détermine la durée de la réverbération, le Pre-Delay, qui définit le délai avant les premières réflexions, et le Dry/Wet, qui contrôle le mélange entre le son original (Dry) et le son réverbéré (Wet).

## VST: ReaVerbate (Cockos)

ReaVerbate (Cockos) est un plugin de réverbération inclus dans REAPER qui permet de simuler la résonance d’un espace virtuel et de contrôler l’ambiance, la profondeur et la spatialisation d’un son.

| Paramètre     | Valeur           |
| ------------- | ---------------- |
| Wet           | ⚙️**Knob**       |
| Dry           | 0 dB             |
| Room Size     | 🎚️**Fader** (60) |
| Dampening     | 55               |
| Stereo Width  | 1.00             |
| Initial Delay | 20 ms            |
| Lowpass       | 10000 Hz         |
| Highpass      | 200 Hz           |

### Wet

> Contrôle le volume du son réverbéré, indépendamment du son original.

- Augmenter le Wet rend la réverbération plus présente et enveloppante, tandis que le diminuer rend le son plus sec et direct. À `-∞ dB`, la réverbération devient inaudible.
- Il n’existe pas de valeur universelle en dB, car le résultat dépend du signal original et de la réverbération utilisée. Sur une piste avec Dry à 0 dB, un Wet entre environ -18 et -8 dB constitue une plage d’essai raisonnable, à ajuster à l’oreille.

### Dry

> Contrôle le volume du signal original, sans réverbération.

- Augmenter le Dry rend l’instrument original plus présent, tandis que le diminuer laisse davantage de place à la réverbération par rapport au son direct. Conserver le Dry à 0 dB préserve le niveau du signal original.
- Le knob Wet suffit alors pour ajouter ou retirer la réverbération sans modifier ce niveau.
- Sur une piste où la réverbération est insérée directement, le Dry est souvent conservé à 0 dB. Sur un bus de réverbération auxiliaire, il est généralement réglé à -∞ dB pour éviter de reproduire le signal original.

### Room Size

> Détermine la taille de l’espace virtuel dans lequel le son résonne.

- Augmenter le Room Size donne l’impression d’un espace plus grand, généralement avec une réverbération plus développée. Le diminuer crée un espace plus petit, avec des résonances plus compactes.
- Une valeur de 60 produit une impression d’espace relativement grand sans être excessivement extrême. La plage 25–85 du fader permet de passer d’une petite salle à une ambiance beaucoup plus vaste, tout en évitant les extrêmes du paramètre.
- Il n’existe pas de référence universelle pour les valeurs numériques de Room Size. Dans ReaVerbate, une plage d’exploration de 40–80 est raisonnable, mais ce sont des valeurs propres au plugin.

### Dampening

> Simule l’absorption du son par les matériaux présents dans une pièce, particulièrement celle des hautes fréquences.

- Augmenter le Dampening rend généralement la réverbération plus sombre et atténue plus rapidement ses hautes fréquences. Le diminuer laisse davantage d’aigus résonner dans l’espace.
- Une valeur de 55 représente un compromis entre une réverbération brillante et une réverbération fortement amortie. Elle permet de conserver une certaine clarté sans produire trop de résonances aiguës.
- Les valeurs ne sont pas standardisées entre les plugins. Une plage de 30–70 constitue un point de départ pratique dans ReaVerbate, mais les producteurs ajustent surtout ce paramètre selon la tonalité recherchée.

### Stereo Width

> Contrôle la largeur stéréo du son réverbéré, c’est-à-dire son étendue entre les haut-parleurs gauche et droit.

- Augmenter la valeur vers 1.00 élargit la réverbération, tandis que la diminuer vers 0 la concentre progressivement en mono. ReaVerbate permet également des valeurs négatives qui inversent la disposition stéréo.
- Une valeur de 1.00 conserve la largeur stéréo normale de la réverbération, ce qui permet de créer une ambiance enveloppante sans manipuler davantage son positionnement.
- Une réverbération large est courante sur les synthétiseurs, les Pads et les Keys. Les réglages proches de la largeur normale sont fréquents, mais une réverbération plus étroite peut être préférable dans un mixage dense.

### Initial Delay

> Détermine le délai entre le son original et le début de la réverbération. Ce paramètre est également appelé Pre-Delay.

- Augmenter le délai sépare davantage l’attaque de la note de sa réverbération, ce qui améliore souvent sa définition. Le diminuer fait commencer la réverbération plus rapidement, créant un son plus fusionné et parfois moins précis.
- Un délai de 20 ms permet de conserver une attaque relativement nette tout en donnant une sensation d’espace. C’est particulièrement utile pour le Lead et les Keys, où la précision des notes demeure importante.
- Des valeurs d’environ 10–40 ms sont fréquentes pour les instruments mélodiques et les réverbérations naturelles. Des délais plus importants, comme 50–100 ms, sont parfois utilisés pour des effets plus prononcés.

### Lowpass

> Filtre les hautes fréquences du signal réverbéré, afin de contrôler la brillance de la réverbération.

- Augmenter la fréquence du Lowpass laisse passer davantage d’aigus dans la réverbération. La diminuer coupe progressivement les fréquences élevées, créant un effet plus sombre et plus doux.
- Une fréquence de 10 000 Hz conserve une bonne partie de la brillance du son tout en atténuant les fréquences très aiguës. Cela évite que la réverbération devienne trop agressive ou envahissante.
- Les filtres Lowpass des réverbérations sont fréquemment réglés entre 6 000 et 12 000 Hz. Des fréquences plus basses peuvent être utilisées pour une réverbération particulièrement sombre ou discrète.

### Highpass

> Filtre les basses fréquences du signal réverbéré afin d’éviter leur accumulation.

- Augmenter la fréquence du Highpass retire davantage de graves de la réverbération, ce qui peut rendre le mixage plus clair. La diminuer laisse davantage de basses fréquences résonner, créant un son plus profond, mais potentiellement plus brouillon.
- Une fréquence de 200 Hz permet de limiter l’accumulation des graves dans la réverbération tout en conservant suffisamment de fréquences moyennes et aiguës pour créer une impression d’espace.
- Les filtres Highpass sur les réverbérations sont couramment placés entre 150 et 350 Hz, parfois davantage dans les mixages particulièrement chargés en basses fréquences.
