# Distorsion

## Définition

La Distorsion (Distortion) est un effet audio (FX) qui modifie la forme d’onde d’un signal sonore, généralement en amplifiant puis en écrêtant (Clipping) certaines parties du signal. Cette transformation génère de nouvelles harmoniques, donnant au son un caractère plus agressif, rugueux, puissant ou métallique. La Distorsion peut être subtile ou extrêmement prononcée, jusqu’à rendre le son original difficile à reconnaître.

## Utilité

La Distorsion permet d’ajouter de la puissance, de l’agressivité et du caractère à un instrument. Elle est particulièrement utilisée sur les guitares électriques, les synthétiseurs Lead, les basses et certaines percussions pour produire des sonorités plus riches, tranchantes ou expérimentales. En production musicale, elle peut également aider un instrument à ressortir dans le mixage en renforçant ses harmoniques, sans nécessairement augmenter son volume.

## Fonctionnement

La Distorsion fonctionne en appliquant un traitement non linéaire au signal audio, qui modifie sa forme d’onde et génère de nouvelles fréquences harmoniques. Ses principaux paramètres sont le Drive (ou Gain), qui détermine l’intensité de la distorsion, le Tone, qui ajuste la couleur sonore, et le Output Level, qui contrôle le volume final. Certains plugins proposent également un Dry/Wet, permettant de mélanger le signal original avec le signal déformé, ainsi que différents types de Clipping, comme le Soft Clipping, plus progressif, et le Hard Clipping, plus agressif.

## JS: Distorsion

JS: Distortion (Cockos) est un plugin audio inclus dans REAPER qui permet de déformer un signal sonore en accentuant ses harmoniques, afin de produire des sonorités plus agressives, rugueuses et saturées.

| Paramètre    | Valeur               |
| ------------ | -------------------- |
| Gain         | 🎚️**Fader** (+12 dB) |
| Hardness     | 6                    |
| Max Volume   | -12 dB               |
| Channel Mode | Stereo               |
| Wet (REAPER) | ⚙️**Knob**           |

### Gain (dB)

> Détermine l’amplification du signal avant sa déformation, ce qui influence directement l’intensité de la distorsion.

- Augmenter : Pousse davantage le signal dans la distorsion, produisant un son plus agressif, dense et riche en harmoniques.
- Diminuer : Réduit l’intensité de la déformation, produisant un son plus propre et plus proche de l’original.
- Une valeur de +12 dB constitue un point de départ pour obtenir une distorsion perceptible sans commencer directement avec les +20 dB de ta capture. Le knob Arturia permet de passer d’un son légèrement déformé à une distorsion beaucoup plus prononcée.
- Le Gain ou Drive est généralement ajusté selon le signal entrant et le type de distorsion. Les amplifications de +6 à +18 dB constituent une plage d’expérimentation utile, mais elles ne produisent pas la même quantité de distorsion sur tous les instruments.

### Hardness

> Contrôle la dureté de la déformation appliquée au signal audio, influençant le caractère de l’écrêtage (Clipping).

- Augmenter : Rend généralement la distorsion plus dure et abrupte, avec un caractère plus agressif et davantage d’harmoniques aiguës.
- Diminuer : Rend la déformation plus progressive et douce, produisant un résultat qui peut se rapprocher d’une saturation.
- Une valeur de 6 permet de conserver le caractère agressif recherché pour ton Lead, sans devoir manipuler simultanément le Gain et la Hardness. C’est le Gain qui servira à modifier l’agressivité en performance.
- Il n’existe pas de valeur standard pour Hardness, puisque cette échelle est propre au plugin. Le principe équivalent est le choix entre un écrêtage progressif (Soft Clipping) et un écrêtage plus abrupt (Hard Clipping).

### Max Volume (dB)

> Définit le niveau maximal autorisé pour le signal traité, afin de limiter son amplitude après la distorsion.

- Augmenter : Autorise un niveau de sortie plus élevé, ce qui peut rendre le signal traité plus fort.
- Diminuer : Abaisse le plafond de sortie et limite davantage les pics, ce qui peut rendre le son moins fort.
- Je conserverais initialement la valeur de -12 dB affichée dans ta capture, puisqu’elle permet de limiter le niveau des signaux fortement déformés. Il faudra toutefois comparer le volume avec et sans effet pour éviter une différence trop importante.
- Aucun plafond n’est universel. En production, on ajuste le niveau de sortie de la distorsion en fonction du reste du mixage, tout en préservant suffisamment de marge avant l’écrêtage numérique. Ce paramètre ne remplace pas nécessairement un véritable Limiter.

### Channel Mode

> Détermine quels canaux audio sont traités par la distorsion et de quelle manière le plugin gère le signal.

- Changer le mode : Le mode Stereo traite les deux canaux du signal, tandis que les modes monophoniques permettent de travailler avec un signal mono selon les options disponibles.
- Le mode Stereo conserve le traitement des deux canaux de tes instruments virtuels, particulièrement utile pour les sons de Keys et de Lead possédant une image stéréo.
- Le traitement mono est courant pour les instruments monophoniques, notamment certaines guitares et basses. Le traitement stéréo convient aux synthétiseurs et aux instruments virtuels produisant un signal stéréo.

### Wet (REAPER)

> Détermine la proportion de signal traité par la distorsion dans le mélange final.

- Paramètre externe au plugin, accessible via le contrôle de mélange Wet de REAPER.
- Augmenter : Rend la distorsion plus présente jusqu’à obtenir uniquement le signal traité.
- Diminuer : Réduit la quantité de distorsion et conserve davantage le son original.
- Cette configuration permet de faire apparaître progressivement la distorsion pendant une performance. Elle est préférable au contrôle du Gain seul, puisque ce dernier influence à la fois la déformation et potentiellement le niveau sonore.
- Les mélanges parallèles sont courants pour conserver la définition du son original. Une plage de 10–50 % peut donner des résultats intéressants, tandis que 100 % est fréquent pour les distorsions utilisées comme sonorité principale. Le niveau perçu doit être surveillé pendant le mélange.
