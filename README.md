# calineos-watchdog

Sentinelle de disponibilité de [calineos.store](https://calineos.store), exécutée toutes les 5 minutes par GitHub Actions.

Elle ne contient aucun code de la boutique ni aucun secret d'hébergement. En cas de panne, elle déclenche le workflow « Surveillance Calineos » du dépôt privé, qui ouvre le ticket d'alerte et relance le VPS si nécessaire.

Secret requis : `CALINEOS_DISPATCH_TOKEN`, un jeton GitHub à accès fin limité au dépôt `calineos` (Actions : lecture et écriture ; Issues : lecture).
