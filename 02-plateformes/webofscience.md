# Web of Science

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | `AND`<br/>`OR`<br/>`NOT` |
| opérateurs<br/>de proximité | `NEAR/`n<br/>`SAME` |
| troncature | `*` (zéro ou plus de caractères)<br/>`?` (un caractère exactement)<br/>`$` (zéro ou un caractère) <br/>*troncature possible à gauche, au milieu et à droite* <br/>*3 caractères minimum doivent être fournis* |
| phrase | `"..."` |
| interprétation<br/>de la requête | oui (lemmatisation et variantes UK/US) |
| historique | oui |

**Exemples**   
`rainbow AND trout AND fish AND farm` est équivalent à `rainbow trout fish farm`, car AND est l'opéateur par défaut.   
`beverage NEAR/5 bottle` renvoie les résultats où "beverage" se trouve à max. 5 mots de "bottle".   
`salmon NEAR virus` renvoie les résultats où "salmon" se trouve à max. 15 mots de "virus" (valeur par défaut).   
`AD=(McGill Univ SAME Quebec SAME Canada)` renvoie les résultats où "McGill Univ" et Quebec et Canada apparaissent dans la même adresse.   
`TS=(cat SAME mouse)` est équivalent à `TS=(cat AND mouse)`, car ailleurs que dans le champs "adresse", SAME est équivalent à AND.   

`s*food` renvoie seafood, soyfood, etc.   
`enzym*` renvoie enzyme, enzymes, enzymatic, enzymic, etc.   
`Hofman*` renvoie Hofman, Hofmann, etc.   
`wom?n` renvoie woman et women.   
`colo$r` renvoie color et colour (notez que les variantes US/UK sont prises en compte sans ça).   
`grain$` renvoie grain et grains.   
`organi?ation*` renvoie organisation, organisations, organisational, organization, organizations, organizational, etc.   

*sources*:   
[Web of Science Core Collection Help](http://images.webofknowledge.com/WOKRS524B8/help/WOS/hp_search.html) (ancienne version, plus facile à utiliser)   
[Search Help](http://webofscience.help.clarivate.com/en-us/Content/advanced-search.html) (nouvelle version, plus... récente)   

Notez que l'aide de la plateforme Web of Science est adaptée à la base de données consultée. Les informations données ci-dessus correspondent à **Web of Science Core Collection**, la base de données native de la plateforme.
