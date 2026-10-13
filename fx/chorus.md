# Chorus

## Définition

Le Chorus est un effet audio qui épaissit un son en donnant l’impression que plusieurs instruments jouent simultanément la même note, avec de légères différences de hauteur et de timing.

## Utilité

Le Chorus permet de rendre un son plus riche, plus large et plus enveloppant. Il est particulièrement utilisé sur les synthétiseurs, les pianos électriques, les guitares et les Pads pour ajouter de la profondeur et du mouvement, sans nécessairement modifier la mélodie.

## Fonctionnement

Le Chorus fonctionne en créant des copies légèrement retardées du son original, dont le délai varie continuellement grâce à une modulation. Ces petites variations produisent des différences de hauteur et de timing qui donnent l’impression que plusieurs sources sonores jouent ensemble. Les copies sont ensuite mélangées au signal original.

## JS: Chorus

JS: Chorus (Cockos) est un plugin d’effet audio inclus dans REAPER qui permet d’épaissir et d’élargir un son en créant plusieurs voix légèrement décalées et modulées en hauteur, donnant l’impression que plusieurs instruments jouent simultanément.

| Paramètre          | Valeur            |
| ------------------ | ----------------- |
| Chorus Length (ms) | 25 ms             |
| Number Of Voices   | 3                 |
| Rate (Hz)          | 0.8 Hz            |
| Pitch Fudge Factor | 🎚️**Fader** (0.7) |
| Wet Mix (dB)       | ⚙️**Knob**        |
| Dry Mix (dB)       | 0 dB              |

### Chorus Length (ms)

> Détermine la durée du court délai appliqué aux copies du son original, exprimée en millisecondes.

- Augmenter la valeur espace davantage les copies du son original, créant un Chorus plus large et détaché. La diminuer rapproche les copies, produisant un effet plus serré qui peut progressivement ressembler à un Flanger.
- Une valeur de 25 ms produit un Chorus suffisamment large pour épaissir le son, sans créer de répétitions clairement distinctes comme un Delay.
- Environ 15–35 ms pour un Chorus classique.

### Number Of Voices

> Détermine le nombre de voix supplémentaires générées par le Chorus pour simuler plusieurs instruments jouant simultanément.

- Augmenter le nombre de voix rend le son plus dense, riche et enveloppant. Le diminuer produit un Chorus plus léger et plus transparent, avec moins de copies du signal.
- Trois voix offrent un bon compromis entre richesse sonore et clarté, particulièrement pour les Keys et les synthétiseurs.
- Environ 2–4 voix pour un Chorus classique. Certains effets de type Ensemble utilisent davantage de voix pour obtenir une texture plus dense.

### Rate (Hz)

> Contrôle la vitesse de modulation des copies sonores, exprimée en Hertz (cycles par seconde).

- Augmenter le Rate accélère les variations de hauteur et de timing, produisant un son plus animé, parfois proche du vibrato. Le diminuer ralentit ces variations, créant un mouvement plus doux et progressif.
- Une valeur de 0,8 Hz crée un mouvement perceptible sans trop déstabiliser les notes. La plage du fader permet de passer d’un Chorus lent et atmosphérique à un effet plus rapide et expressif.
- Environ 0,3–1,2 Hz pour un Chorus traditionnel, avec des valeurs supérieures pour des effets plus prononcés.

### Pitch Fudge Factor

> Contrôle la profondeur de modulation de hauteur des voix générées. Ce paramètre correspond approximativement au _Depth_ présent sur d’autres plugins de Chorus.

- Augmenter la valeur accentue les variations de hauteur et rend le Chorus plus prononcé, voire légèrement désaccordé. La diminuer réduit ces variations pour obtenir un effet plus subtil et stable.
- Une valeur de 0,7 apporte suffisamment de modulation pour rendre le Chorus audible, sans exagérer les variations de hauteur.
- Ce paramètre est propre au plugin et ne possède pas de plage industrielle standard. Les autres Chorus utilisent généralement un contrôle Depth, souvent réglé à une intensité modérée pour éviter un effet de désaccordage trop important.

### Wet Mix (dB)

> Contrôle le volume des voix générées par le Chorus, indépendamment du son original.

- Augmenter le Wet Mix rend le Chorus plus présent, épais et enveloppant. Le diminuer réduit l’effet jusqu’à retrouver uniquement le son original.
- Cette plage permet de passer d’un son complètement sec à un Chorus clairement perceptible. Une valeur initiale de -10 dB offre un enrichissement sonore sans trop masquer le caractère original de l’instrument.
- Les Chorus proposent souvent un mélange Wet/Dry exprimé en pourcentage, avec des valeurs typiques de 20–50 % pour un effet modéré. Avec un Dry à 0 dB, environ -15 à -6 dB de Wet constitue un point de départ pratique, sans être directement équivalent à ces pourcentages.

### Dry Mix (dB)

> Contrôle le volume du signal original, sans les modifications produites par le Chorus.

- Augmenter le Dry Mix renforce la présence du son original, tandis que le diminuer laisse davantage de place aux voix modulées.
- Une valeur de 0 dB conserve le niveau original de l’instrument. Le Wet Mix permet alors d’ajuster l’intensité du Chorus sans devoir modifier le volume du signal direct.
- Le Dry est généralement conservé à 0 dB lorsque le Chorus est inséré directement sur une piste. Sur un bus auxiliaire, il est normalement réglé à -∞ dB.
