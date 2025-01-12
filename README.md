
Les fonctionnalités principales : 
  #1. void afficherMenu()
Description :
Cette fonction affiche un menu simple pour interagir avec le système de gestion des voitures.
Elle présente quatre options :

Ajouter une voiture.
Afficher les voitures disponibles.
Rechercher une voiture par marque.
Quitter le programme.
L'utilisateur doit entrer un choix parmi ces options.

 #2. void ajouterVoiture(FILE *file)
Description :
Cette fonction permet d'ajouter les informations d'une voiture au fichier spécifié.

Étapes :
L'utilisateur est invité à entrer les détails de la voiture :
ID
Marque
Modèle
Type de carburant
Nombre de places
Type de transmission (automatique ou manuelle)
Prix par jour
Disponibilité (1 = disponible, 0 = non disponible).
Ces informations sont ensuite enregistrées dans le fichier sous forme de ligne formatée (CSV).
Résultat : Les informations de la voiture sont sauvegardées, et un message de confirmation est affiché.
 #3. void afficherVoitures(FILE *file)
Description :
Cette fonction lit les informations des voitures stockées dans le fichier et affiche uniquement les voitures marquées comme disponibles.

Étapes :
Le fichier est lu ligne par ligne.
Les voitures disponibles (champ "disponible" égal à 1) sont affichées avec leurs détails :
ID, Marque, Modèle, Type de carburant, Nombre de places, Transmission, Prix par jour.
Résultat : Les informations des voitures disponibles sont affichées dans la console.
 #4. void rechercherVoiture(FILE *file)
Description :
Cette fonction permet de rechercher des voitures par marque dans le fichier spécifié.

Étapes :
L'utilisateur entre le nom de la marque qu'il souhaite rechercher.
Le fichier est parcouru ligne par ligne, et les voitures correspondant à cette marque sont affichées avec leurs détails.
Si aucune voiture ne correspond, un message d'erreur est affiché.
Résultat :
Affiche les voitures correspondant à la marque recherchée .
