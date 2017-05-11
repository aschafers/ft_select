# FT_SELECT

Ce projet a pour but de prendre un ensemble d'arguments passés en paramètres à
la commande ./ft_select et vous permet de sélectionner un ou plusieurs éléments
sur une ou plusieurs pages à retourner.


Exemple:
```
./ft_select /usr/bin/*
```
![Exemple](https://cloud.githubusercontent.com/assets/27807971/25771382/80e0beac-324f-11e7-80b1-bda7eab49bcc.png)


## Installation

```
git clone --recursive git@github.com:aschafers/ft_select.git
```
```
make
```


## Usage:

Permet de supprimer les fichiers qui seront sélectionnés.
```
rm `./ft_select /usr/bin/*`
```

Permet d'afficher certains fichiers.
```
cat `./ft_select /usr/bin/*`
```

Permet de git add certains fichiers.
```
cat `./ft_s
```
Comme vous l'aurez compris, les possibilités sont infinies.

## Contrôles:

| Commandes principales                  | Actions                                       |
| ---------------------------------------|-----------------------------------------------|
| Espace                                 | Permet de selectionner un élément.            |
| Enter                                  | Permet de retourner les éléments selectionnés.|
| Echap                                  | Permet de quitter sans rien retourner.        |
| Up (flèche du haut)                    | permet de reculer d'un élément.               |
| Right (flèche de droite)               | Permet d'avancer d'une colonne.               |
| Left (flèche de gauche)                | Permet de reculer d'une colonne.              |
| Down (flèche du bas)                   | Permet d'avancer d'un élément.                |
| Del (touche del ou fn + retour arrière)| Permet de suprimer un élément de la liste.    |


# Infos supplémentaires

### Espace:
  Permet de sélectionner ou désélectionner un élément.
  Et avance d'un élément.
### Up:
  Permet de reculer d'un élément. Si vous vous trouvez sur 
  le premier élément, vous place sur le dernier. Vous permet
  aussi de reculer de page en page si vous êtes sur le premier
  élément de la page. Pour finir, si vous vous trouvez sur le premier 
  élément de la première page, vous serez placé sur le dernier élément de la dernière page.
### Right:
  Permet d'avancer de colonne en colonne. Si vous êtes sur l'élément 2 de la première 
  commande, vous serez déplacé sur le même élément de la prochaine colonne. Si la colonne 
  cible a moins d'élements que l'index actuel de votre élément, vous serez placé sur
  le dernier élément de la prochaine colonne. Si vous êtes sur la dernière colonne de la page, vous serez
  déplacé sur la prochaine page au même index. Et si vous êtes sur la dernière colonne de la dernière 
  page vous reviendrez à la première colonne de la première page.
### Left:
  Même comportement que right mais inversé.
### Down:
  Même comportement que up mais inversé.
### Recherche:
  La recherche se lance en tapant un caractère. Une loupe devrait apparaître en bas de la fenêtre avec votre recherche.
  Il suffit d'appuyer sur entrer pour aller à la première occurrence. Rappuyer sur entrer aura pour effet d'aller à la prochaine
  occurrence et ainsi de suite. Si vous vous trouvez sur la dernière occurrence, vous serezs ramené à la première.
  Pour sortir de la recherche, il vous suffit de taper sur la touche supprimer, ce qui aura pour effet de supprimer la dernière lettre
  de la recherche. Quand plus aucune lettre n'est dans la recherche vous repassez en mode normal.
### Del:
  Permet de supprimer un élément de la liste. La suppression ne supprimera pas les fichiers de votre ordinateur.
 


