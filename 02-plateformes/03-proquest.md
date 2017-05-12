# ProQuest

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*, N/*n*<br/>PRE/*n*, P/*n*, - |
| troncature | * (zéro ou plus de caractères)<br/>? (un caractère)<br/>$n, [\*n]<br/> *troncature possible au milieu et à droite*<br/>\< *date*<br/>\> *date*<br/>\<= *date*<br/>\>= *date*<br/>*date*-*date* |
| phrase | EXACT("..."), X("...") |
| interprétation<br/>de la requête | oui (*stemming* et variantes UK/US) |
| historique | oui |

**Exemples**   
`nursing NEAR education` renvoie les résultats où "nursing" se trouve à max. 4 mots de "education" (valeur par défaut).   
`nursing NEAR/3 education` renvoie les résultats où "nursing" se trouve à max. 3 mots de "education". Idem pour `nursing N/3 education` (en utilisant l'opérateur N, vous devez fournir un nombre).   
`nursing PRE/3 education` renvoie les résultats où "nursing" précède "education" de 3 mots max. Idem pour `nursing P/3 education`.   
`enseignement-infirmier` (**avec un tiret**) correspond à `enseignement PRE/0 infirmier` ou `enseignement P/0 infirmier`.   

`nurse?` renvoie nurses, nursed, etc.   
`sm?th` renvoie smith et smyth.   
`ad???` renvoie added, adult, adopt, etc.   
`nurse*` renvoie nurse, nurses, nursed, etc.   
`colo*r` renvoie colour et color.   
`*old` renvoie told, household, bold, etc. (max. 10 caractères)   
`[*5]beat` renvoie upbeat, downbeat, offbeat, heartbeat, etc. (ajoute max. 5 caractères comme préfixe). Idem pour `$5beat`.   
`nutr[*5]` renvoie nutrition, nutrient, nutrients, etc. (ajoute max. 5 caractères comme suffixe). Idem pour `nutr$5`.   
`YR(2005-2008)` renvoie les résultats des publications de 2005 à 2008.   

`EXACT("higher education")` renvoie le  résultats contenant l'expression exacte "higher education" (ni plus ni moins).   
`SU.EXACT("higher education")` renvoie les résultats dont le sujet est "higher education" en exculant p. ex. "higher education funding".   

*source*: [ProQuest Help - Search Tips](http://search.proquest.com/help/academic/webframe.html?Search_Tips.html)

