# Delay

## Définition

Le Delay est un effet audio qui consiste à répéter un son après un certain délai, créant ainsi un effet d’écho. Contrairement à la Reverb, qui produit une multitude de réflexions rapprochées simulant un espace acoustique, le Delay génère des répétitions généralement distinctes et perceptibles du son original.

## Utilité

Le Delay permet d’ajouter de la profondeur, du rythme et du mouvement à un son. Il peut créer de simples échos, donner l’impression que plusieurs instruments jouent ensemble ou produire des ambiances complexes et atmosphériques. En production musicale, il est particulièrement utilisé sur les voix, les guitares et les synthétiseurs pour enrichir le son sans nécessairement le rendre plus volumineux.

## Fonctionnement

Le Delay fonctionne en enregistrant temporairement le signal audio pour le rejouer après un intervalle déterminé, exprimé en millisecondes ou synchronisé au tempo musical. Plusieurs paramètres permettent de modifier cet effet, notamment le Time, qui détermine le temps entre les répétitions, le Feedback, qui contrôle le nombre de répétitions et leur diminution progressive, et le Dry/Wet, qui ajuste le mélange entre le son original (Dry) et les échos (Wet). Certains Delays permettent également de modifier la tonalité ou la position stéréo des répétitions.

## VST: ReaDelay (VST)

ReaDelay est un plugin de Delay inclus dans REAPER, qui permet de créer des échos simples ou complexes grâce à plusieurs répétitions configurables (taps).

| Paramètre        | Valeur               |
| ---------------- | -------------------- |
| Wet              | ⚙️**Knob**           |
| Dry              | 0 dB                 |
| Enabled          | true                 |
| Solo Active Tap  | false                |
| Length (time)    | 0 ms                 |
| Length (musical) | 2.00 × ⅛             |
| Feedback         | 🎚️**Fader** (-10 dB) |
| Lowpass filter   | 6000 Hz              |
| Hipass filter    | 200 Hz               |
| Resolution       | 24 bits              |
| Stereo width     | 1.00                 |
| Volume (tap)     | 0 dB                 |
| Pan (tap)        | 0.000                |

### Wet

> Contrôle le volume global des échos générés par ReaDelay, indépendamment du son original.

- Augmenter le Wet rend les échos plus présents et perceptibles, tandis que le diminuer les rend plus discrets. À -∞ dB, aucun écho n’est audible.
- Cette plage permet de passer d’un son complètement sec à des échos bien présents. La valeur initiale de -10 dB offre un bon équilibre entre le son original et les répétitions.
- Pour un Delay inséré directement sur une piste, environ -18 à -8 dB constitue une plage de départ raisonnable. Il n’existe cependant pas de valeur universelle, car le résultat dépend du signal et du nombre de répétitions.

### Dry

> Contrôle le volume du son original, sans les échos.

- Augmenter le Dry rend le son original plus présent, tandis que le diminuer laisse davantage de place aux échos.
- Une valeur de 0 dB conserve le volume original de l’instrument. Le Wet peut alors être manipulé indépendamment sans diminuer le signal direct.
- 0 dB est courant pour un Delay inséré directement sur une piste. Sur un bus auxiliaire dédié au Delay, le Dry est généralement réglé à -∞ dB.

### Enabled

> Active ou désactive le tap sélectionné, c’est-à-dire une ligne de Delay possédant ses propres paramètres.

- Activer ce paramètre permet au tap de produire ses échos, tandis que le désactiver le rend inactif.
- Le tap doit rester activé pour produire l’effet. Le knob Wet permet déjà de rendre les échos inaudibles lorsque nécessaire.
- Les taps utilisés sont normalement activés. Ceux qui ne servent pas peuvent être désactivés.

### Solo Active Tap

> Permet d’écouter uniquement le tap sélectionné lorsque plusieurs taps sont présents.

- Activer cette option isole le tap sélectionné, tandis que la désactiver permet à tous les taps activés de fonctionner ensemble.
- Notre configuration utilise un seul tap pour commencer. Cette option est donc inutile en performance et doit rester désactivée.
- Le Solo est principalement utilisé pendant la conception ou l’ajustement d’un Delay complexe à plusieurs taps.

### Length (time)

> Détermine le délai temporel en millisecondes avant qu’un écho soit entendu.

- Augmenter la valeur espace davantage les échos dans le temps, tandis que la diminuer les rapproche du son original. Les délais très courts peuvent produire un effet d’épaississement plutôt qu’un écho distinct.
- Nous utiliserons plutôt Length (musical) pour synchroniser les répétitions au tempo du projet. Conserver Length (time) à 0 ms évite d’ajouter un décalage temporel supplémentaire.
- Pour un Delay non synchronisé, environ 70–150 ms est courant pour un slapback, tandis que 200–600 ms permet des échos plus espacés. Une valeur de 0 ms est appropriée lorsqu’on utilise exclusivement la synchronisation musicale.

### Length (musical)

> Détermine l’intervalle entre les échos selon le tempo du projet, exprimé en fractions de notes musicales.

- Augmenter la valeur espace les répétitions en utilisant des durées musicales plus longues. La diminuer produit des répétitions plus rapides et rapprochées.
- Une valeur de 2.00 représente deux croches, donc une noire (1/4 de note). Ce réglage permet d’obtenir des répétitions bien synchronisées avec le rythme de la musique, sans être trop rapides.
- Les durées de 1/8, 1/8 pointée et 1/4 de note sont très courantes pour les Delays rythmiques. Les valeurs de 1/2 note et plus sont souvent utilisées pour des effets atmosphériques.

### Feedback

> Contrôle la quantité de signal réinjectée dans le Delay après chaque répétition, ce qui détermine combien de temps les échos continuent.

- Augmenter le Feedback vers 0 dB produit davantage de répétitions, qui diminuent plus lentement en volume. Le diminuer réduit leur nombre et les fait disparaître plus rapidement.
- Une valeur de -10 dB permet d’obtenir plusieurs échos audibles qui diminuent naturellement en intensité. La plage du fader permet de passer d’un écho presque unique à des répétitions plus persistantes, sans approcher trop près du Feedback à 0 dB, qui pourrait entretenir les échos indéfiniment.
- Le Feedback est souvent exprimé en pourcentage dans les autres plugins. Une réinjection d’environ 15–50 % est un point de départ courant, correspondant approximativement à -16,5 à -6 dB en amplitude. Les effets expérimentaux peuvent employer des valeurs beaucoup plus élevées.

### Lowpass Filter

> Atténue les hautes fréquences des échos afin de contrôler leur brillance.

- Augmenter la fréquence du Lowpass laisse passer davantage d’aigus, produisant des échos plus brillants. La diminuer rend les répétitions plus sombres et plus douces.
- Une fréquence de 6 000 Hz permet aux échos de conserver une bonne intelligibilité tout en réduisant leur brillance. Ils restent ainsi légèrement en arrière-plan par rapport au son original.
- Les filtres Lowpass sur les Delays sont fréquemment placés entre 3 000 et 10 000 Hz. Des fréquences plus basses sont utilisées pour reproduire les caractéristiques de certains Delays analogiques ou à bande.

### Hipass Filter

> Atténue les basses fréquences des échos pour éviter qu’elles s’accumulent dans le mixage.

- Augmenter la fréquence du Highpass retire davantage de graves des répétitions, tandis que la diminuer permet aux échos de conserver un son plus profond et plus riche en basses.
- Une fréquence de 200 Hz empêche une partie des basses fréquences de se répéter inutilement, laissant davantage de place aux instruments graves comme la Bass et le Kick.
- Les Delays sont souvent filtrés entre 150 et 400 Hz dans les basses fréquences. Des valeurs plus élevées peuvent être utilisées pour obtenir des échos particulièrement légers.

### Resolution

> Définit la résolution numérique des échos, exprimée en bits, et influence leur fidélité sonore.

- Augmenter la résolution conserve un son plus fidèle et précis. La diminuer introduit davantage de bruit de quantification et de distorsion numérique, créant un effet Lo-Fi.
- Une résolution de 24 bits préserve la qualité sonore des échos. Puisque nous disposons déjà d’effets de destruction et de Bit Reduction sur l’AKAI, il n’est pas nécessaire d’en ajouter au Delay.
- Les résolutions de 16 à 24 bits sont courantes pour les Delays numériques propres. Les résolutions de 8 à 12 bits peuvent être utilisées volontairement pour créer des effets Lo-Fi.

### Stereo Width

> Contrôle la largeur stéréo des échos, c’est-à-dire leur répartition entre les haut-parleurs gauche et droit.

- Augmenter la largeur vers 1.00 élargit l’image stéréo, tandis que la diminuer vers 0 concentre progressivement les échos au centre.
- Une valeur de 1.00 conserve la largeur stéréo normale du Delay, offrant une sensation d’espace sans modifier artificiellement la position des répétitions.
- Les Delays stéréo larges sont courants sur les Keys, les Pads et les synthétiseurs. Une image stéréo plus étroite est parfois préférable lorsqu’un mixage contient déjà beaucoup d’éléments panoramiques.

### Volume (Tap)

> Contrôle le volume du tap sélectionné, indépendamment du niveau Wet global.

- Augmenter le volume rend les échos de ce tap plus présents, tandis que le diminuer les atténue. Avec plusieurs taps, chacun peut posséder son propre volume.
- Une valeur de 0 dB conserve le niveau normal du tap. Puisque nous utilisons un seul tap, il est plus simple de contrôler l’intensité générale avec le Wet.
- Dans un Delay à plusieurs taps, leurs volumes peuvent être ajustés individuellement, souvent avec des atténuations de quelques décibels. Avec un seul tap, 0 dB est un réglage de départ approprié.

### Pan (Tap)

> Détermine la position gauche ou droite des échos produits par le tap sélectionné.

- Déplacer le Pan vers la droite positionne davantage les échos dans le canal droit, tandis que le déplacer vers la gauche les positionne dans le canal gauche.
- Conserver le Pan au centre permet de maintenir un équilibre entre les canaux gauche et droit. Avec un seul tap, ce réglage est généralement suffisant.
- Le Pan central est courant pour un Delay simple. Les Delays créatifs et Ping-Pong utilisent souvent plusieurs taps positionnés alternativement à gauche et à droite.
