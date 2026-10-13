# Limiter

> Le Limiter est un processeur dynamique qui empêche les pics sonores de dépasser un plafond défini.

Le Limiter fonctionne comme un compresseur à ratio très élevé, conçu pour limiter les pics du signal audio lorsqu’ils atteignent un seuil précis. Il est principalement utilisé pour contrôler les crêtes excessives, éviter l’écrêtage numérique et maîtriser le niveau de sortie d’un mixage. Contrairement à un compresseur traditionnel, qui réduit progressivement la dynamique, le Limiter applique une réduction beaucoup plus importante lorsqu’un signal dépasse son seuil.

## Variation

- **Augmenter la limitation.** Contrôle davantage les pics, mais peut écraser la dynamique et provoquer de la distorsion.
- **Diminuer la limitation.** Préserve davantage les transitoires et la dynamique, mais laisse passer des pics plus élevés.

## Contrôle

Statique, généralement sur le Master ou un bus nécessitant une protection particulière.

## Utilité

Faible sur chaque instrument individuellement, mais potentiellement utile sur le Master. Je ne recommande pas d’ajouter un Limiter systématiquement à chacune de tes pistes. Il ne remplace pas une bonne gestion des niveaux et ne protège pas contre toutes les saturations possibles.
