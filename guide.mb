# Dinobarriere — Guide

Plugin permettant aux entreprises autorisées par le staff de vendre des barrières automatiques : l'employé pose une barrière, place des points au sol, et la barrière s'ouvre toute seule quand un véhicule autorisé roule dessus, puis se referme après 10 secondes. En option, une caméra surveille l'entrée : à chaque véhicule qui passe, un message (embed) est envoyé sur le Discord du propriétaire avec le modèle, la couleur et la plaque, pour savoir qui est entré. Les installations sont sauvegardées à chaque redémarrage.

---

## 1. Commandes

### `/dinobarrieresetup` — Staff
Réglages du plugin : entreprises autorisées, prix, webhook Discord, liste des installations.

### `/listebarriere` — Staff
Liste des installations. On peut s'y téléporter ou les supprimer.

### `/setupbarriere` — Employé
- **Créer une barrière** : type → caméra → propriétaire (nom prénom) → paiement.
- **Liste des barrières** : voir ou supprimer celles de l'entreprise.

| Barrière | Prix en plus |
|---|---|
| Barrière levante | 799 € |
| Barrière levante 7 m | 1799 € |
| Barrière levante (sans support) | 799 € |

Caméras : Caméra d'extérieur ou Caméra 360°.
Prix total = prix de base + barrière + caméra (si choisie).

### `/pointbarriere` — Employé
À faire quand la barrière et la caméra sont posées (moins de 10 m entre elles).
Place **1 ou 2 points** au sol, à pied, à moins de 10 m de la barrière (un de chaque côté). L'installation est terminée au 2e point.

### `/mesbarriere` — Propriétaire
- **Mode ouvert** : tous les véhicules ouvrent.
- **Mode fermé** : seuls le propriétaire et les copropriétaires (ou leurs véhicules) ouvrent.
- **Copropriétaires** : ajouter par nom prénom ou ID, retirer.
- **Webhook caméra** : si l'installation a une caméra.

---

## 2. Bon à savoir

- Si l'employé abandonne, se déconnecte ou si le serveur redémarre avant la fin : remboursement et objets repris (sauf si déjà posés sur la carte).
- Caméra : à chaque véhicule qui passe, un embed Discord (modèle, couleur, plaque) est envoyé sur le webhook du propriétaire, réglé dans `/mesbarriere`. 30 % des plaques sont illisibles.
- Le staff reçoit un embed quand une installation est terminée.

---

## 3. Configuration

Fichiers créés au premier démarrage dans le dossier `dinoBarriere/`, à côté du `.dll`.

### `config.json`

| Réglage | Défaut | Rôle |
|---|---|---|
| `NiveauStaffMinimum` | `3` | Niveau staff pour les commandes staff |
| `PrixSuppression` | `-1` | Prix de suppression (`-1` = prix de base) |
| `PourcentagePlaqueIllisible` | `30` | % de plaques illisibles |
| `DelaiFermetureSecondes` | `10` | Délai avant fermeture |
| `MaxInstallationsEnCoursParEmploye` | `3` | Installations non terminées max |
| `DistanceMaxEntreObjets` | `10` | Distance max barrière ↔ caméra (m) |
| `MaxPointsParBarriere` | `2` | Points max par barrière |
| `DistanceMaxPointBarriere` | `10` | Distance max point ↔ barrière (m) |
| `DistanceRecherchePoseObjets` | `30` | Distance max employé ↔ objets posés (m) |
| `DistanceMaxSuppression` | `15` | Distance max pour supprimer (m) |
| `DelaiEntreEnvoisCameraSecondes` | `30` | Délai entre deux envois caméra (même véhicule) |

### `settings.json`
Modifié en jeu par le staff : entreprises autorisées, prix de base (5000), prix caméra (2500), webhook staff.

`installations.json` : les installations. `dinoBarriere_log.txt` : le journal.

---

## 4. Dépendance obligatoire

### ModKit

Dinobarriere nécessite **ModKit** pour fonctionner.

Téléchargement de ModKit :
https://plugins.modnl.me/plugins

---

## 5. Support

Si vous avez des questions ou rencontrez un problème avec le plugin, vous pouvez contacter :

Discord : py0ui
Serveur discord : https://discord.gg/2cwRtZTjM5 et ou https://discord.gg/KnRR4GYpQV
