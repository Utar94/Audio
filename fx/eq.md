# EQ

## Définition

L’égalisation (EQ, Equalization) est un traitement audio qui permet d’ajuster l’intensité de différentes fréquences d’un son. Elle sert à modifier son équilibre tonal en augmentant ou en diminuant certaines bandes de fréquences, comme les graves (Bass), les médiums (Mid) et les aigus (Treble). L’EQ est considéré comme un effet audio (FX), même s’il appartient plus précisément à la catégorie des traitements de correction et de mixage plutôt qu’aux effets créatifs comme la Reverb ou le Chorus.

## Utilité

L’EQ permet d’améliorer la clarté, l’équilibre et la définition d’un instrument en ajustant les fréquences qui le composent. Il peut rendre un son plus chaleureux, brillant, profond ou précis, mais aussi éliminer les fréquences indésirables. En production musicale, il est particulièrement utile pour éviter que plusieurs instruments occupent trop les mêmes fréquences, par exemple en réduisant les graves des Keys pour laisser davantage de place à la Bass.

## Fonctionnement

L’EQ fonctionne à l’aide de filtres qui amplifient ou atténuent certaines fréquences du signal audio. Ses principaux paramètres sont la Frequency, qui détermine la fréquence ciblée, le Gain, qui contrôle son amplification ou son atténuation en décibels, et le Q (Bandwidth), qui définit la largeur de la bande de fréquences affectée. Différents types de filtres, comme le Highpass, le Lowpass, le Bell et le Shelf, permettent de modifier précisément le spectre sonore selon les besoins du mixage.

## VST: ReaEQ (Cockos)

ReaEQ est un égaliseur paramétrique inclus dans REAPER qui permet d’amplifier, d’atténuer ou de filtrer différentes fréquences d’un signal audio afin d’en modifier l’équilibre tonal, la clarté et le caractère sonore.

### Type

> Détermine le type de filtre appliqué à la bande sélectionnée et la manière dont il modifie les fréquences du son.

- Il ne s’agit pas d’une valeur que l’on augmente ou diminue, mais d’un choix entre plusieurs types de filtres. Le type de filtre doit être choisi selon le problème à corriger ou le résultat sonore souhaité. Le modifier pendant une performance pourrait transformer radicalement le son.

Les filtres les plus couramment utilisés sont High Pass, Low Pass, Band (Bell), Low Shelf et High Shelf.

- **High Pass (HPF).** Atténue les fréquences graves sous une fréquence choisie, tout en laissant passer les fréquences aiguës. Utile pour éliminer les graves inutiles.
- **Low Pass (LPF).** Atténue les fréquences aiguës au-dessus d’une fréquence choisie, tout en laissant passer les graves. Utile pour adoucir un son trop brillant.
- **Band (Bell / Peak).** Amplifie ou atténue une plage de fréquences autour d’une fréquence centrale. C’est le filtre le plus polyvalent pour corriger ou enrichir un instrument.
- **Low Shelf.** Amplifie ou atténue progressivement l’ensemble des fréquences graves sous un certain point. Utile pour ajuster la chaleur ou la profondeur du son.
- **High Shelf.** Amplifie ou atténue progressivement l’ensemble des fréquences aiguës au-dessus d’un certain point. Utile pour ajuster la brillance.
- **Notch.** Atténue fortement une plage très étroite de fréquences. Utile pour supprimer une résonance gênante ou un sifflement.
- **Band Pass.** Laisse passer une plage de fréquences et atténue celles situées au-dessus et en dessous. Utile pour créer des sons filtrés ou des effets de type radio.
- **All Pass.** Laisse passer toutes les fréquences sans modifier directement leur niveau, mais change leur phase. Utile pour des traitements particuliers de phase.

### Frequency (Hz)

> Détermine la fréquence sur laquelle le filtre agit, exprimée en Hertz.

- Augmenter : Déplace la fréquence ciblée vers les aigus.
- Diminuer : Déplace la fréquence ciblée vers les graves.
- L’effet audible dépend du type de filtre. Par exemple, augmenter la fréquence d’un High Pass élimine davantage de graves, tandis qu’augmenter celle d’un Low Pass laisse passer davantage d’aigus.
- La fréquence doit être choisie selon les caractéristiques de chaque instrument et sa place dans le mixage. Une valeur fixe permet de conserver un équilibre sonore constant pendant la performance.

Les fréquences habituellement travaillées couvrent l’ensemble du spectre audible, approximativement de 20 à 20 000 Hz. Les zones les plus courantes sont :

| Fréquences       | Caractéristiques                          |
| ---------------- | ----------------------------------------- |
| 20–60 Hz         | Sub-bass, vibrations profondes            |
| 60–250 Hz        | Graves, puissance, chaleur                |
| 250–500 Hz       | Bas-médiums, corps, son parfois brouillon |
| 500–2 000 Hz     | Médiums, caractère et définition          |
| 2 000–5 000 Hz   | Présence, attaque, précision              |
| 5 000–10 000 Hz  | Brillance, détails                        |
| 10 000–20 000 Hz | Air, éclat, hautes fréquences             |

### Gain (dB)

> Contrôle l’amplification ou l’atténuation des fréquences ciblées par un filtre compatible, comme Band ou Shelf.

- Augmenter : Amplifie les fréquences ciblées, rendant cette partie du spectre plus présente.
- Diminuer : Atténue les fréquences ciblées, réduisant leur importance dans le son.
- À 0 dB, un filtre Bell ou Shelf ne produit aucune amplification ou atténuation.
- Partir de 0 dB permet de préserver le caractère original de la banque de sons. Les ajustements doivent ensuite être effectués uniquement lorsqu’une fréquence doit être corrigée ou mise en valeur.
- Industrie : Des ajustements de ±1 à 3 dB sont courants pour des corrections subtiles. Des modifications de ±3 à 6 dB peuvent être nécessaires pour des interventions plus importantes.
- Le Gain de bande ne fonctionne pas de la même façon sur tous les types de filtres. Sur un Low Pass ou un High Pass, la fréquence de coupure est généralement le réglage principal.

### Bandwidth (oct)

Rôle : Détermine la largeur de la plage de fréquences affectée par un filtre, exprimée en octaves.

- Augmenter : Élargit la plage de fréquences affectée, permettant une correction plus générale et progressive.
- Diminuer : Rétrécit la plage, permettant une correction plus précise et ciblée.
- Une largeur de 1,50 octave constitue un bon point de départ pour effectuer des corrections musicales relativement douces sans cibler des fréquences trop étroites.
- Environ 1–3 octaves pour les corrections larges, et 0,1–1 octave pour les corrections plus chirurgicales. Le choix dépend du type de filtre et du problème à résoudre.

### Enabled

> Active ou désactive individuellement la bande sélectionnée.

- Activé : Le filtre influence le signal audio selon ses paramètres.
- Désactivé : Le filtre est ignoré et n’affecte plus le son.
- Les bandes inutilisées peuvent être désactivées pour simplifier la configuration et éviter des traitements superflus.
- Les ingénieurs activent uniquement les bandes nécessaires. Il n’est pas obligatoire d’utiliser toutes les bandes disponibles dans un EQ.

### Output Gain (dB)

> Contrôle le volume global du signal traité par ReaEQ, après l’application de l’ensemble des bandes.

- Augmenter : Augmente le volume global du signal après égalisation.
- Diminuer : Réduit le volume global du signal après égalisation.
- Une valeur de 0 dB évite d’ajouter une amplification inutile. Si l’EQ modifie sensiblement le volume perçu, ce contrôle peut servir à compenser cette différence pour comparer équitablement le son traité au son original.
- Le gain de sortie est souvent ajusté pour conserver un niveau perçu similaire avant et après égalisation. Il n’existe pas de valeur fixe universelle.

### Log-scale Automated Frequencies

> Modifie la manière dont les fréquences sont représentées dans les paramètres d’automatisation REAPER, en utilisant une échelle logarithmique plutôt que linéaire.

- Activé : Répartit les fréquences de façon plus adaptée à leur perception musicale, facilitant notamment les ajustements dans les graves.
- Désactivé : Utilise une échelle linéaire, dans laquelle les basses fréquences occupent proportionnellement moins d’espace.
- L’échelle logarithmique facilite les éventuelles automatisations de fréquences, même si nous n’en prévoyons pas pour l’instant. Elle ne modifie pas directement le son.
- Les représentations logarithmiques des fréquences sont courantes dans les outils audio, puisqu’elles correspondent mieux à la perception musicale des hauteurs.

### Paramètres d’interface

Ces options ne modifient pas directement le son.

| Paramètre      | Fonction                                                    | Recommandation         |
| -------------- | ----------------------------------------------------------- | ---------------------- |
| Metering       | Choisit les signaux affichés par les indicateurs de niveau. | All                    |
| Show Tabs      | Affiche les onglets des bandes.                             | Activé                 |
| Show Grid      | Affiche la grille de fréquences et de décibels.             | Activé                 |
| Show Phase     | Affiche la réponse en phase des filtres.                    | Désactivé initialement |
| Add Band       | Ajoute une bande d’égalisation.                             | Au besoin              |
| Remove Band    | Supprime une bande.                                         | Au besoin              |
| Reset Defaults | Réinitialise les paramètres.                                | Au besoin              |

### Configuration selon tes instruments

Contrairement aux autres FX, je ne recommande pas un seul preset ReaEQ identique pour tous tes instruments.

Voici des points de départ adaptés à ton organisation Bass / Keys / Pad / Lead. Ils supposent que ces instruments jouent leurs rôles habituels, et devront être ajustés aux sons réellement utilisés.

| Instrument | High Pass suggéré   | Autres corrections                                                             |
| ---------- | ------------------- | ------------------------------------------------------------------------------ |
| Bass       | 25–35 Hz, au besoin | Réduire les fréquences brouillonnes vers 200–350 Hz si nécessaire              |
| Keys       | 60–100 Hz           | Réduire légèrement les bas-médiums si les Keys masquent la Bass                |
| Pad        | 100–200 Hz          | Atténuer certaines fréquences moyennes si le Pad masque les autres instruments |
| Lead       | 80–150 Hz           | Ajuster la présence vers 2–5 kHz si le Lead manque de définition               |

Ces fréquences ne sont pas des règles absolues. Par exemple, si ton Lead utilise des notes très graves, un High Pass trop élevé pourrait retirer une partie importante de son son.

#### Exemple de configuration ReaEQ pour les Keys

| Bande | Type       | Frequency | Gain | Bandwidth                        |
| ----- | ---------- | --------- | ---- | -------------------------------- |
| 1     | High Pass  | 80 Hz     | —    | Ajuster selon la pente souhaitée |
| 2     | Band       | 300 Hz    | 0 dB | 1,50 oct                         |
| 3     | Band       | 2 500 Hz  | 0 dB | 1,50 oct                         |
| 4     | High Shelf | 8 000 Hz  | 0 dB | 1,50 oct                         |
| 5     | Low Pass   | Désactivé | —    | —                                |

Avec les bandes 2 à 4 à 0 dB, ces dernières ne modifient pas le son initialement. Elles restent disponibles si une correction devient nécessaire. Seul le High Pass agit réellement dans cet exemple.

### Résumé des affectations MIDI

| Paramètre                       | AKAI     | Arturia  | Valeur initiale    |
| ------------------------------- | -------- | -------- | ------------------ |
| Type                            | Statique | Statique | Selon la bande     |
| Frequency                       | Statique | Statique | Selon l’instrument |
| Gain (bande)                    | Statique | Statique | 0 dB               |
| Bandwidth                       | Statique | Statique | 1,50 oct (Bell)    |
| Enabled                         | Statique | Statique | Selon la bande     |
| Output Gain                     | Statique | Statique | 0 dB               |
| Log-scale Automated Frequencies | Statique | Statique | Activé             |

#### Pourquoi aucun knob ni fader ?

L’EQ sert principalement à corriger et équilibrer les fréquences des instruments dans le mixage. Une fois les ajustements effectués, il est préférable de les conserver constants pour éviter de déséquilibrer le son pendant une performance.

Il existe une exception intéressante : le Filter, un effet créatif qui permet de balayer les fréquences en temps réel. Même s’il repose sur des principes similaires à l’EQ, son objectif est différent. Nous pouvons donc conserver ReaEQ statique et continuer à utiliser un Filter contrôlé par ton joystick AKAI, comme prévu dans ton setup.

Conclusion : ReaEQ est utile pour tes quatre instruments, mais aucun de ses paramètres n’a besoin de monopoliser un knob ou un fader MIDI.
