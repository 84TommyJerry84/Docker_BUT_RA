# Guide d'Utilisation du Dockerfile

## Renommer le Dockerfile avant utilisation

Avant de commencer à utiliser ce projet pour créer vos conteneurs Docker, vous devez effectuer une petite modification. Le fichier `Dockerfile` fourni contient un numéro dans son nom, par exemple : `Dockerfile1`, `Dockerfile2`, etc. Pour que les builds Docker fonctionnent correctement, vous devez renommer ce fichier en `Dockerfile` sans numéro.

### Étapes pour renommer le Dockerfile :

1. Ouvrez le répertoire du projet.
2. Localisez le fichier nommé `Dockerfile1`, `Dockerfile2`, ou similaire.
3. Renommez le fichier en supprimant le numéro afin qu'il soit simplement nommé `Dockerfile`.
   
   Exemple :
   - **Avant :** `Dockerfile1`
   - **Après :** `Dockerfile`

### Exécuter le build après renommage :

Une fois le fichier correctement renommé, vous pouvez lancer le build Docker comme suit :

```bash
docker build -t nom_de_votre_image .
