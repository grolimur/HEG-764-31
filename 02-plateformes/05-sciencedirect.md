# ScienceDirect

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>AND NOT |
| opérateurs<br/>de proximité | W/*n*<br/>PRE/*n* |
| troncature | * (zéro ou plus de caractères)<br/>? (un caractère) <br/>*troncature possible à gauche, au milieu et à droite* |
| phrase | "..."<br/>{...} |
| interprétation<br/>de la requête | oui |
| historique | oui |

**Exemples**   
`pain W/15 morphine` renvoie les résultats où "pain" se trouve à max. 15 mots de "morphine".   
`behavioural PRE/3 disturbances` renvoie les résultats où "behavioural" précède "disturbances" de 3 mots max.   

`h*rt` renvoie hurt, heart, etc.   
`h*r*t` renvoie heart, harvest, homograft, hypervalent, etc.   
`gro?t` renvoie grout, groat, etc. mais pas groundnut p. ex.   
`transplant??` renvoie transplanted et transplanter.   
`?ight` renvoie light, right, eight, fight, might, etc.   
`"heart attack"` est équivalent à `"heart-attack"`, car le tiret est ignoré.   
`"criminal* insan*"` renvoie "criminally insane", "criminal insanity", etc.   
`{heart-attack}` est différent de `{heart attack}`, car le tiret est pris en compte.   

Remarques:   
1. la requête `bay W/6 ship PRE/0 channel` n'est pas valide. Elle doit s'écrire `(bay W/6 ship) AND (ship PRE/0 channel)` pour être comprise par ScienceDirect.   
2. `coronary W/2 circadian W/5 rhythm` va en fait chercher `coronary W/5 circadian W/5 rhythm` , car seule la dernière valeur de *n* est prise en compte.   

*source*: [ScienceDirect WebHelp](http://help.sciencedirect.com)

