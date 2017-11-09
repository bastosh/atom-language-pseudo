# atom-pseudo-fr
Atom package to highlight french pseudo-code || Educational purpose  
Based on https://atom.io/users/TheoMessin pseudo-code language package

This version of pseudo-code is used at CNAM PACA

## File format
```.sdo``` ```.pseudo```

## Installation
```
cd ~/.atom/packages  
git clone https://github.com/bastosh/atom-pseudo-fr.git
```
Restart Atom and you're good to go!  
![restart](https://github.com/bastosh/atom-pseudo-fr/blob/master/img/restart.png?raw=true)

## Conventions
### Mots-clés
```
Procédure
Fonction
Var
Vars
Tableau
Structure
Début
Fin
Si
Sinon
FinSi
Pour
TantQue
FinTantQue
Suivant
Pas de
Booléen
Vrai
Faux
Numérique (42, 3.14, -2) // Utilisation du point pour les décimaux
Caractère ('x') // Guillemets simples
Chaîne de caractères ("We will rock you") // Guillemets doubles
NON
ET
OU
XOR
Renvoyer
```
```
// Optionnel pour affiner le type Numérique
Entier // pour les nombres entiers
Réel // pour les nombres décimaux
```

### Opérateurs
```
<- // affectation
+ // addition
- // soustraction
* // multiplication
/ // division
^ // puissance
<= // inférieur ou égal
>= // supérieur ou égal
= // égal à
<> // différent de
& // concaténation
```

### Commentaires
```
// Commentaire sur une ligne

/* Commentaire
   sur plusieurs
   lignes */
```

### Tableaux
```
Tableau notes(6) en Numérique
Var premiereNote en Numérique
premiereNote <- 12
notes(0) <- premiereNote
```

### Structures
#### Variables structurées
```
Structure Annuaire
  Nom en Chaîne de caractères
  Prenom en Chaîne de caractères
  Tel en Chaîne de caractères
  Mail en Chaîne de caractères
Fin Structure

Var Personne en Annuaire

// Méthode d'assignation n°1
Personne <- “Durand”, “Pierre”, “0442012345”, "pierredurand@truc.com"

// Méthode d'assignation n°2
Personne.Nom <- “Durand”
Personne.Prenom <- “Pierre”
Personne.Tel <- “0442012345”
Personne.Mail <- "pierredurand@truc.com"
```
#### Tableaux structurés
```
annuaire(N).Nom
annuaire(N).Prenom
annuaire(N).Tel
annuaire(N).Mail
```

#### Fontions prédéfinies
```
Lire(nombreSaisi)
Écrire("Hello World!")
```
```
Ent(Numérique) // Renvoie la partie entière d'un nombre
Alea() // Renvoie un nombre aléatoire entre 0 et 1
Len(chaîne) // Renvoie la longueur d'une chaîne de caractères
Mid(chaîne,n1,n2) // Renvoie un extrait de la chaîne, commençant au caractère n1 et faisant n2 caractères de long
Left(chaîne,n) // Renvoie les n caractères les plus à gauche dans chaîne
Right(chaîne,n) // Renvoie les n caractères les plus à droite dans chaîne
Find(chaîne1,chaîne2) // Renvoie un nombre correspondant à la position de chaîne2 dans chaîne1. Si chaîne2 n’est pas comprise dans chaîne1, la fonction renvoie zéro
```

### Fonctions
#### Déclaration
```
Fonction faireQuelqueChose(param1, param2)
Début
  <insctructions>
  Renvoyer <resultat>
Fin
```

## Aperçu (monokai theme)

![capture1](https://github.com/bastosh/atom-pseudo-fr/blob/master/exemples/capture1.png?raw=true "Pseudo-code syntax highlight")

![capture2](https://github.com/bastosh/atom-pseudo-fr/blob/master/exemples/capture2.png?raw=true "Pseudo-code syntax highlight")

![capture3](https://github.com/bastosh/atom-pseudo-fr/blob/master/exemples/capture3.png?raw=true "Pseudo-code syntax highlight")
