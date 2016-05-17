# SpringerLink

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND, &<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*<br/>ONEAR/*n*  |
| troncature | milieu - droite<br/>* (zéro ou plus de caractères)<br/>? (un caractère) |
| phrase | "..." |
| interpréation<br/>de la requête | stemming |
| historique | ? |

**Exemples**   
*information **NEAR/4** systems* renvoie les résultats où "information" se trouve à max. 4 mots de "system".   
*system **NEAR** testing* renvoie les résultats où "system" se trouve à max. 10 mots de "testing" (valeur par défaut).   
Idem pour *system **ONEAR** testing*.   
*system **ONEAR/2** testing* renvoie les résultats où "system" précède "testing" de 2 mots max.   

**hea*** renvoie head, heats, health, heated, heating, etc.   
**hea?** renvoie head, heat, heal, etc.   

