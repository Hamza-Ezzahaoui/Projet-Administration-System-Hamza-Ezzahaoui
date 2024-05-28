Todo List Application

Cette application en C permet de gérer une liste de tâches. Vous pouvez créer, mettre à jour, supprimer, afficher et rechercher des tâches ainsi que les lister par date d'échéance. Les tâches sont stockées dans un fichier texte `tasks.txt`.

 Compilation

Pour compiler le programme, utilisez la commande suivante :


gcc -o todo main.c

 Utilisation

Le programme offre plusieurs commandes pour gérer vos tâches. Voici un aperçu des commandes disponibles :

 Créer une tâche

todo create <titre> --due_date <YYYY-MM-DD> [--description <desc>] [--location <loc>]


Mettre à jour une tâche


todo update <id> [--title <titre>] [--description <desc>] [--location <loc>] [--due_date <YYYY-MM-DD>] [--completed <0|1>]


Supprimer une tâche


todo delete <id>

Afficher une tâche


todo show <id>


Lister les tâches


todo list [--date <YYYY-MM-DD>]

 Rechercher une tâche par titre


todo search <titre>


 Aide

Pour afficher l'aide et les commandes disponibles :


todo


 Format du fichier `tasks.txt`

Le fichier `tasks.txt` contient les tâches avec le format suivant :

id|titre|description|location|due_date|completed


 Exemples

 Créer une nouvelle tâche


todo create "Acheter du lait" --due_date "2024-06-01" --description "Acheter du lait au supermarché" --location "Supermarché"


 Mettre à jour une tâche


todo update 1 --title "Acheter du lait et du pain" --completed 1


 Supprimer une tâche


todo delete 1

Afficher une tâche


todo show 1


Lister les tâches pour une date spécifique


todo list --date "2024-06-01"


 Rechercher une tâche par titre


todo search "lait"


