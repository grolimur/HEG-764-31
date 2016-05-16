# Web of Science
(anciennement Web of Knowledge)

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*<br/>SAME |
| troncature | gauche - milieu - droite<br/>* (zéro ou plus de caractères)<br/>? (un caractère)<br/>$ (zéro ou un caractère) |
| phrase | "..." |
| interpréation<br/>de la requête | lemmatisation<br/>variantes UK/US |
| historique | oui |

**Exemples**   
*salmon **NEAR/10** virus* renvoie les résultats où "salmon" se trouve à max. 10 mots de "virus".   
*salmon **NEAR** virus* renvoie les résultats où "salmon" se trouve à max. 15 mots de "virus" (valeur par défaut).   
*AD=(McGill Univ **SAME** Quebec **SAME** Canada)* renvoie les résultats où "McGill Univ" et Quebec et Canada apparaissent dans l'adresse (SAME est l'équivalent de AND, mais dans le champs "adresse").   

**s*food** renvoie seafood, soyfood, etc.   
**enzym*** renvoie enzyme, enzymes, enzymatic, enzymic, etc.   
**Hofman*** renvoie Hofman, Hofmann, etc.   
**wom?n** renvoie woman et women.   
**colo$r** renvoie color et colour (notez que les vairantes US/UK sont prises en compte sans ça).   
**grain$** renvoie grain et grains.   
**organi?ation*** renvoie organisation, organisations, organisational, organization, organizations, organizational, etc.   
