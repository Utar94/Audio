# Ring Modulation

## Définition

La Ring Modulation est un effet audio (FX) qui transforme la tonalité d’un son en combinant son signal avec celui d’un oscillateur appelé Carrier (porteuse). Elle produit de nouvelles fréquences qui n’étaient pas nécessairement présentes dans le son original, créant des sonorités métalliques, robotiques, dissonantes ou futuristes. Contrairement au Chorus ou au Flanger, qui modifient principalement la perception du son par des décalages temporels, la Ring Modulation transforme directement son contenu fréquentiel.

## Utilité

La Ring Modulation permet de créer des textures sonores inhabituelles et expérimentales, particulièrement sur les synthétiseurs Lead, les guitares et les percussions. Elle est souvent utilisée pour produire des sons de cloches métalliques, des voix robotiques, des effets de science-fiction ou des distorsions complexes. À faible intensité et avec une fréquence de modulation basse, elle peut aussi produire des pulsations proches du Tremolo, tandis qu’à forte intensité elle peut rendre un instrument presque méconnaissable.

## Fonctionnement

La Ring Modulation fonctionne en multipliant le signal audio original par celui d’un oscillateur, généralement une onde sinusoïdale. Cette multiplication génère de nouvelles fréquences correspondant principalement à la somme et à la différence des fréquences des deux signaux, ce qui produit les sonorités caractéristiques de l’effet. Ses principaux paramètres sont la Mod Frequency, qui contrôle la fréquence de l’oscillateur, le Feedback, qui peut accentuer la complexité du traitement, et le Mix, qui détermine la proportion entre le son original et le son modulé.

## JS: Ring Modulator (Cockos)

JS: Ring Modulator (Cockos) est un plugin audio inclus dans REAPER qui permet de transformer un son par modulation en anneau, en générant de nouvelles fréquences pour produire des textures métalliques, robotiques et expérimentales, avec des contrôles de fréquence, de feedback, de non-linéarité et de mixage.

| Paramètre       | Valeur           |
| --------------- | ---------------- |
| Processing      | Stereo           |
| Mod Input Diode | Off              |
| Mod Frequency   | 🎚️**Fader** (40) |
| Feedback        | 0%               |
| Non-Linearities | 10%              |
| Mix             | ⚙️**Knob**       |
| Output          | 0 dB             |
| Oversample x2   | On               |

### Processing

> Détermine si le plugin traite le signal en mode Mono ou Stereo.

- Le mode Stereo permet de traiter les deux canaux du signal stéréo. Le mode Mono utilise un traitement monophonique.
- Le mode Stereo est préférable pour préserver le caractère stéréo de tes banques de sons et des instruments utilisant des effets spatiaux.
- Les deux modes sont utilisés. Stereo convient généralement aux synthétiseurs stéréo, tandis que Mono est fréquent pour les sources monophoniques.

### Mod Input Diode (Waveshaper)

> Ajoute une transformation non linéaire au signal de modulation, ce qui modifie sa forme d’onde et les harmoniques produites.

- Activer le Waveshaper transforme la porteuse et peut générer des textures plus complexes, métalliques ou agressives. Le désactiver conserve une modulation sinusoïdale plus classique.
- Je recommande de commencer avec une Ring Modulation classique, sans transformation supplémentaire. Les sonorités métalliques seront déjà possibles avec le paramètre Mod Frequency.
- Une porteuse sinusoïdale est courante pour la Ring Modulation traditionnelle. Les Waveshapers sont davantage utilisés pour le sound design et les effets expérimentaux.

### Mod Frequency (Scale)

> Contrôle la fréquence de l’oscillateur qui module le signal original, déterminant en grande partie la texture sonore produite.

- Augmenter : Produit généralement des fréquences supplémentaires plus espacées, créant des sonorités métalliques, robotiques ou dissonantes.
- Diminuer : Rapproche les nouvelles fréquences des fréquences originales. Aux valeurs très basses, l’effet peut ressembler à un Tremolo.
- Une valeur de 40 correspond à environ 321 Hz dans ta capture, ce qui produit une modulation suffisamment rapide pour créer des textures métalliques. La plage 20–60 permet d’explorer différents caractères sans utiliser toute l’étendue du plugin.

La fréquence de modulation varie considérablement selon l’effet recherché :

| Fréquence réelle | Effet généralement obtenu                                     |
| ---------------- | ------------------------------------------------------------- |
| 1–20 Hz          | Pulsations proches du Tremolo                                 |
| 20–100 Hz        | Modulation rugueuse, vibrations rapides                       |
| 100–500 Hz       | Sonorités robotiques et métalliques                           |
| 500–2 000 Hz     | Textures dissonantes, sons de cloches et effets expérimentaux |

Important : Le paramètre Scale n’est pas directement exprimé en Hz. Il faut regarder l’indication `MOD F` au bas du plugin pour connaître la fréquence réelle.

### Feedback (%)

> Contrôle la quantité de signal traité qui est réinjectée dans le Ring Modulator pour être modulée à nouveau.

- Augmenter : Renforce les transformations successives, créant davantage d’harmoniques, de complexité et potentiellement de distorsion.
- Diminuer : Réduit ces transformations, produisant un effet plus simple et prévisible.
- À 0 %, le signal ne subit pas de réinjection supplémentaire. Puisque la Ring Modulation transforme déjà fortement le son, je recommande de commencer sans Feedback pour éviter une texture trop agressive.
- Aucun standard universel. Un Feedback faible ou nul est courant pour une modulation simple; les valeurs plus élevées sont surtout utilisées pour créer des effets expérimentaux.

### Non-Linearities (%)

> Introduit de petites variations dans la fréquence de modulation et le Feedback, créant un comportement moins régulier.

- Augmenter : Rend la modulation plus instable, irrégulière et potentiellement chaotique.
- Diminuer : Stabilise progressivement le traitement, produisant une modulation plus constante et prévisible.
- Une valeur de 10 % introduit une légère instabilité sans trop altérer le caractère du son. Elle permet d’obtenir une texture un peu moins mécanique.
- Ce paramètre n’est pas standardisé. Les modulations classiques utilisent généralement une fréquence stable, tandis que les effets expérimentaux peuvent introduire davantage d’instabilité.

### Mix (%)

> Contrôle la proportion entre le son original (Dry) et le son traité par la Ring Modulation (Wet).

- Augmenter : Rend la Ring Modulation plus présente, transformant progressivement le son original en une texture métallique ou robotique.
- Diminuer : Réduit l’intensité de l’effet et conserve davantage le caractère original de l’instrument.
- La Ring Modulation peut transformer radicalement un instrument. Une plage de 0–70 % permet d’obtenir des effets très prononcés tout en évitant les réglages entièrement Wet, qui peuvent rendre la mélodie difficile à reconnaître.
- Il n’existe pas de valeur standard. Un mélange de 10–30 % constitue un point de départ pratique pour conserver une bonne partie du son original. Les valeurs de 50–100 % conviennent davantage aux transformations sonores importantes.

### Output (-inf/+40dB)

> Contrôle le niveau de sortie du signal après l’application de la Ring Modulation.

- Augmenter : Amplifie le signal traité, pouvant provoquer une saturation si le niveau devient excessif.
- Diminuer : Réduit le niveau de sortie pour éviter que l’effet domine les autres instruments.
- Une valeur de 0 dB évite toute amplification supplémentaire. Le niveau devra toutefois être vérifié, car la Ring Modulation peut modifier le volume perçu même avec un Output à 0 dB.
- Le gain de sortie est généralement ajusté pour obtenir un volume perçu similaire lorsque l’effet est activé ou désactivé. Il n’existe pas de valeur universelle.

### Oversample (x2)

> Permet d’effectuer le traitement audio à une fréquence d’échantillonnage interne deux fois plus élevée afin de réduire certains artefacts numériques.

- Activé : Peut réduire l’Aliasing, particulièrement lorsque la modulation génère des fréquences aiguës, mais augmente la consommation du processeur.
- Désactivé : Réduit la charge du processeur, au risque de produire davantage d’artefacts numériques dans certains cas.
- Je recommande d’activer l’Oversampling x2 puisque la Ring Modulation peut créer de nombreuses fréquences supplémentaires. Cela peut améliorer la propreté du signal, particulièrement avec des modulations rapides.
- L’Oversampling x2 et x4 est courant pour les traitements générant beaucoup d’harmoniques, comme la Distortion, la Saturation et certains effets de modulation. Son utilisation dépend du processeur disponible et de l’amélioration sonore obtenue.
