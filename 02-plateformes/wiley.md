# Wiley Online Library

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | `AND`, `&`, `+`<br/>`OR`<br/>`NOT`, `-` |
| opérateurs<br/>de proximité | - |
| troncature | `*` (zéro ou plus de caractères)<br/>`?` (un caractère exactement)<br/>*troncature possible au milieu et à droite* |
| phrase | `"..."` |
| interprétation<br/>de la requête | oui |
| historique | oui |

**Exemples**   
`spinal cord` est équivalent à `spinal AND cord`.   
`"spinal cord"` ne renvoie que les résultats où l'expression apparaît exactement ainsi.   

`wom?n` renvoie women ou woman.   
`plant*` renvoie tous les mots avec la même racine (ex. plant, plants, planting).   
`an*mia` renvoie les variantes avec une ou plusieurs lettres (ex. anemia, anaemia).   
La troncature ne peut pas être utilisée au début d'un mot-clé (ex. \*tension) ou dans une expression exacte (ex. "tobacco smok\*").

*source*: [Advanced Search - Wiley Online Library](https://onlinelibrary.wiley.com/search/advanced)
