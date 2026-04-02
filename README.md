# Jeu-Du-Loto-Python
<img width="1846" height="957" alt="image" src="https://github.com/user-attachments/assets/084a6bd3-4b6d-49f1-8729-ac4e809b13a9" />

_____________________________________________________________________________________________________________________________________________________________________________________________________________________________
<strong> ~ PRÉSENTATION ~ <strong>

Projet transversal qui a comme objectif de créer un jeu de loto en langage python. Le but est d'allier nos cours de Python et nos cours d'algorithmie pour permettre d'affiner nos compétences et de créer un mini-jeu 
fonctionnel.


~ LES ATTENDUS DU PROJET ~

Les attendues étaient :
- Générer un tirage aléatoire de 10 numéros de loto
- Permettre à l’utilisateur de saisir ses propres numéros
- Comparer les résultats
- Calculer un score
- Attribuer une récompense en fonction du nombre de numéros gagnants


~ DÉMONSTRATION ~

Le jeu se joue sur la console de l'IDE. Succèssivement, s'affiche une entrée où nous devons y taper une valeur comprise entre 1 et 49. Une fois les 10 valeurs rentrées au fur et à mesure, l'algo du jeu va importer de 
manière aléatoire 10 valeurs, les comparer, puis afficher les valeurs de l'utilisateur et les valeurs du "import random". Puis, les valeurs sont comparés et selon le nombre de numéro identique, un petit prix de victoire 
s'affiche.


~ EXPLICATION DU CODE ~

<img width="222" height="27" alt="image" src="https://github.com/user-attachments/assets/502325f4-64c5-43ff-9050-62d541398353" />


"import random" permet donc de générer les 10 numéros aléatoires compris entre 1 et 49.

<img width="694" height="194" alt="image" src="https://github.com/user-attachments/assets/4deaa6e8-893f-47d5-b429-b2e8a1353df7" />


Fonction permettant le résultat en appelant l'"import random" et en affichant les 10 valeurs.

<img width="785" height="630" alt="image" src="https://github.com/user-attachments/assets/62f79354-9535-4c00-9363-d6fb38c7da20" />


Permet d'affiche succèssivement les 10 valeurs à entrer, et la structure conditionnelle sert à vérifier que la valeur entrée est comprise entre 1 et 49, si le nombre a déjà été saisi ou non et si l'entrée est un entier. 
Si les conditions sont respectées, la valeur est ajoutée à la liste "user_nums"

<img width="801" height="308" alt="image" src="https://github.com/user-attachments/assets/8ed46af7-563f-4602-90d6-7306c6be0ca0" />


Cette fonction compare les numéros de l'utilisateur avec le tirage officiel en deux temps. D'abord, elle identifie les numéros gagnants en vérifiant quels chiffres de l'utilisateur sont présents dans la liste de la 
banque. Ensuite, elle calcule un bonus d'ordre en comparant les index de positions de chaque numéro pour voir s'ils ont été saisis dans le même ordre que le tirage.

<img width="769" height="795" alt="image" src="https://github.com/user-attachments/assets/36ea82ff-3966-4025-9985-390f3bed1922" />


Cette fonction gère l'affichage final et l'attribution des lots. Elle compte le nombre de bons numéros pour déterminer le gain du joueur selon trois paliers (grand prix, prix intermédiaire ou petit prix).

<img width="731" height="439" alt="image" src="https://github.com/user-attachments/assets/be23c530-87a2-4c92-8cf9-0aed369d5ec6" />


La fonction main est le chef d’orchestre qui coordonne l’exécution du programme en appelant les autres fonctions dans l’ordre. Elle gère le flux de données : de la génération du tirage et la saisie utilisateur vers le 
calcul des résultats, puis l'affichage des récompenses.


<img width="305" height="57" alt="image" src="https://github.com/user-attachments/assets/84c38655-d7e6-40a1-b6a0-3b139d825552" />


Ces lignes sécurisent le code et indique à Python de ne lancer le jeu uniquement si le fichier est exécuter directement, elle empêche le programme de démarrer si on décide d'importer ces fonctions dans un autre script.


~ PERSPECTIVES À AMÉLIORER ~

1. Afficher le jeu avec une interface graphique :
  → Grâce à une fenêtre (en important la librairie "Tkinter"), nous pouvons afficher le jeu sous une vraie forme de mini-jeu avec une grille, et des animations lors des numéros gagnants.
