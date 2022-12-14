## project_c : chiffrement du perroquet
Projet c pour la formation C/C++ embarqué

```
compilation via le makefile : make
```

```
suppression des fichiers de lien et de l'exécutable : make mrproper
```

```
suppression des fichiers .o : make clean
```

```
génération d'un zip : make zip
```

```
exécution du projet : ./manage_cypher
```

# Thème :

On souhaite à partir d’un fichier source, faire en sorte de le crypter en utilisant l’algorithme du « perroquet ».
Cet algorithme repose sur un mot (le perroquet) qui permet de crypter en calculant la différence ASCII caractère par caractère.
Illustration du principe du perroquet :

```
Mot source à crypter : Olivier
```

```
Perroquet : abcd
```


# Résultat en calcul ascii : 

```c++
(‘O’-‘a’)(‘l’-‘b’)(‘i’-‘c’)(‘v’-‘d’)(‘i’-‘a’)(‘e’-‘b’)(‘r’-‘c’)
```

# Résultat

Concaténation des codes ASCII


# Contraintes : 

L’utilisateur devra lui-même définir son propre perroquet.

Celui qui crypte et qui décrypte doit donc connaître le mot (ou la phrase) du « perroquet ». 

On prévoira donc un fichier 

```
(« peroq.def ») 
```

contenant la chaine de caractères du perroquet.

# On disposera de 2 fichiers :

```
Source (« source.txt ») : 
```
contenant le texte à crypter

```
Résultat (« dest.crt ») : 
```

contenant le texte crypté

# Option :

De plus, on prévoira de supprimer la source après cryptage de telle manière à ne conserver que le fichier crypté.

# Menu

Dans le menu nous avons 8 choix : 

```
1. Chiffrer un texte
2. Dechiffrer un texte
3. Chiffrer par saisi de cle
4. Dechiffrer par saisi de cle
5. Chiffrer par saisi des paths des fichiers
6. Dechiffrer par saisi des paths des fichiers
7. Supprimer le fichier source
8. Voir une demo
0. Quitter

```

# Détails des choix du menu

```
1. Un fichier nommé source.txt contenant le texte clair et un fichier peroq.def contenant la clé  
   de chiffreement sont lus et le chiffré est déposé dans le fichier dest.crt

2. Un fichier nommé dest.crt contenant le texte chiffré et un fichier peroq.def contenant la clé 
   de déchiffreement sont lus et le déchiffré est déposé dans le fichier source.txt

3. La clé de chiffrement est saisie manuellement par l'utilisateur.
4. La clé de déchiffrement est saisie manuellement par l'utilisateur.
5. Les chemins vers les fichiers clair et crypté ainsi que la clé de chiffrement sont saisis 
   manuellement par l'utilisateur.
6. Les chemins vers les fichiers clair et crypté ainsi que la clé de déchiffrement sont saisis 
   manuellement par l'utilisateur.
7. Suppression du fichier source.txt
8. Trois exemples sont donnés pour voir les entrées et sorties dans le cas du chiffrement et 
   du déchiffrement
0. Quitter le programme

```

# Note

```
Dans le cas 1 et 2, les chemins des différents fichiers sont renseignés dans le fichier file.h. 
Ils peuvent être modifiés à volonté.

Les développements et les tests sont réalisés en totalité sous codeBlocks sous windows 10

Les tests en ligne de commande sont réalisés sur Debian 11
```

# La console du programme

![My Image](./pictures/demo.jpg)

# Exécution de la démo

![My Image](./pictures/demo_02.jpg)
