# Bitcrusher

## Définition

Le Bitcrusher est un effet audio (FX) de dégradation numérique qui réduit volontairement la qualité dun signal sonore pour lui donner un caractère granuleux, artificiel et rétro (Lo-Fi). Contrairement à la Distorsion et à la Saturation, qui déforment principalement la forme donde du signal, le Bitcrusher altère sa précision numérique. Il permet notamment de reproduire certaines caractéristiques sonores des anciennes consoles de jeux vidéo, des premiers ordinateurs et des équipements audio numériques à faible résolution.

## Utilité

Le Bitcrusher permet de transformer un son propre et précis en une texture numérique rugueuse, agressive ou expérimentale. Il est particulièrement utilisé sur les synthétiseurs, les percussions, les basses et les instruments électroniques pour créer des sonorités rétro, robotiques ou volontairement dégradées. Selon son intensité, il peut ajouter une légère coloration Lo-Fi ou détruire presque complètement le caractère original dun instrument, ce qui le rend particulièrement intéressant pour le sound design.

## Fonctionnement

Le Bitcrusher fonctionne principalement en réduisant la Bit Depth, qui détermine le nombre de niveaux damplitude disponibles pour représenter le signal numérique, et parfois le Sample Rate, qui détermine le nombre déchantillons audio traités par seconde. Diminuer la Bit Depth introduit des erreurs de quantification, créant du bruit et de la distorsion numérique, tandis que réduire le Sample Rate peut produire des artefacts daliasing et des sonorités plus artificielles. Certains plugins proposent également un Dry/Wet, permettant de mélanger le signal original avec le signal dégradé afin de contrôler lintensité de leffet.

## VST3: BitCrusher (SocaLabs)

BitCrusher (SocaLabs) est un plugin de dégradation numérique qui permet de réduire la résolution et la fréquence d’échantillonnage d’un signal audio, afin de produire des sonorités Lo-Fi, granuleuses, rétro ou volontairement détruites.

| Paramètre    | Valeur                |
| ------------ | --------------------- |
| Bits         | 🎚️**Fader** (12 bits) |
| Rate         | 12 000 Hz             |
| Dirty        | Off                   |
| Wet (REAPER) | ⚙️**Knob**            |

### Bits

> Détermine la résolution numérique du signal en réduisant le nombre de bits utilisés pour représenter son amplitude.

- Augmenter : Améliore la précision du signal, réduit la distorsion numérique et conserve davantage de détails.
- Diminuer : Réduit le nombre de niveaux d’amplitude disponibles, produisant du bruit de quantification, des textures granuleuses et une distorsion de plus en plus prononcée.
- Une résolution de 12 bits donne une coloration Lo-Fi perceptible sans nécessairement rendre le son méconnaissable. La plage de 8 à 16 bits permet de passer d’une dégradation importante à un traitement beaucoup plus discret.
- Les résolutions de 12 et 8 bits sont particulièrement associées aux anciens samplers et équipements numériques. Les résolutions de 4 bits et moins sont généralement utilisées pour des destructions sonores beaucoup plus extrêmes.

### Rate

> Détermine la fréquence d’échantillonnage effective du traitement, c’est-à-dire le nombre de fois par seconde où le signal est actualisé.

- Augmenter : Conserve davantage de détails temporels et réduit les artefacts liés à la réduction de fréquence d’échantillonnage.
- Diminuer : Rend le son plus artificiel et rugueux, avec des artefacts numériques, notamment de l’aliasing lorsque celui-ci n’est pas supprimé.
- Une fréquence de 12 000 Hz permet d’obtenir une texture numérique rétro sans utiliser les fréquences extrêmement basses qui déforment radicalement le son. Je privilégie le contrôle Bits sur l’Arturia pour éviter de devoir manipuler simultanément deux paramètres de dégradation.
- Les anciennes technologies numériques utilisaient différentes fréquences d’échantillonnage, souvent bien inférieures aux 44 100 ou 48 000 Hz actuels. Pour une coloration Lo-Fi, environ 8 000 à 22 050 Hz constitue une plage d’expérimentation intéressante.

### Dirty

> Détermine si le Bitcrusher utilise un traitement numérique brut ou un traitement avec réduction des artefacts d’aliasing.

- On : Désactive les traitements anti-aliasing, produisant un son plus brut, rugueux et potentiellement agressif.
- Off : Utilise un traitement plus propre, qui réduit certains artefacts numériques indésirables tout en conservant l’effet Bitcrusher.
- Je recommande de commencer avec Dirty désactivé, particulièrement puisque tu avais remarqué des bruits numériques désagréables avec ton ancien Bitcrusher. Tu conserveras la dégradation produite par Bits et Rate sans ajouter autant d’aliasing.
- Il n’existe pas de réglage universel. Un traitement propre est intéressant pour une coloration Lo-Fi contrôlée, tandis qu’un traitement brut convient aux effets expérimentaux, chiptune et aux destructions numériques.

### Wet (REAPER)

> Contrôle la quantité de signal traité par le Bitcrusher dans le mélange final.

- Paramètre externe au plugin, accessible dans REAPER.
- Augmenter : Rend la dégradation numérique plus présente.
- Diminuer : Conserve davantage le son original.
- Le Wet permet de faire apparaître progressivement la dégradation sans modifier directement Bits et Rate. C’est également une bonne façon de retrouver un son propre lorsque le contrôle revient à 0 %.
- Un mélange de 10–40 % peut servir à ajouter une légère texture numérique. Les valeurs de 50–100 % conviennent davantage aux effets très marqués et expérimentaux.
