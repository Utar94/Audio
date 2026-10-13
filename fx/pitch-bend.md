# Pitch Bend

## Définition

Le Pitch Bend est une fonction de modulation qui permet de modifier progressivement la hauteur (Pitch) d’une note vers les graves ou les aigus, sans changer la touche jouée. Contrairement au Vibrato, qui fait osciller automatiquement la hauteur autour de la note originale, le Pitch Bend permet au musicien de contrôler directement cette variation, généralement à l’aide d’une roue ou d’un joystick sur un clavier MIDI.

## Utilité

Le Pitch Bend permet d’ajouter de l’expressivité et du réalisme à un instrument en créant des glissements de hauteur entre les notes. Il est particulièrement utilisé sur les synthétiseurs Lead, les guitares virtuelles et les instruments à vent pour reproduire des techniques comme les Bends, les Slides et les Glissandos. Il peut également servir à créer des effets sonores expérimentaux, comme des montées rapides ou des descentes dramatiques de hauteur.

## Fonctionnement

Le Pitch Bend fonctionne en envoyant des messages MIDI qui indiquent au synthétiseur de modifier la hauteur des notes jouées. La position centrale de la roue ou du joystick correspond à la hauteur originale, tandis que les déplacements vers le haut ou le bas augmentent ou diminuent progressivement cette hauteur. L’amplitude maximale de la variation est déterminée par le Pitch Bend Range, généralement exprimé en demi-tons (semitones), avec une valeur courante de ±2 demi-tons, mais pouvant être configurée à ±12 ou ±24 demi-tons selon l’instrument. Contrairement à la Mod Wheel, le contrôle de Pitch Bend revient généralement automatiquement au centre lorsqu’il est relâché.
