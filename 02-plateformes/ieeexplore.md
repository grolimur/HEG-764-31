# IEEE Xplore

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*<br/>ONEAR/*n* |
| troncature | \* (zéro ou plusieurs caractères)<br/>*troncature possible à gauche, au milieu et à droite* |
| phrase | "..." |
| interprétation<br/>de la requête | oui (*stemming* et variantes UK/US) |
| historique | oui |

**Exemples**   
`implantable NEAR/3 cardiac` renvoie les résultats où "implantable" se trouve à max. 3 mots de "cardiac".   
`implantable ONEAR/3 cardiac` renvoie les résultats où "implantable" précède "cardiac" de 3 mots max.   

`electro*` renvoie electron, electrons, electronic, electronics, electromagnetic, electromechanical, electrostatic, etc.   
`*optic` renvoie optic,fiber-optic, electrooptic, acoustooptic, etc.   
`me*n` renvoie men, mean, median, etc.   

`"computer"` renvoie computer exactement (pas computers)

*source*: [IEEE Xplore Global Search](http://ieeexplore.ieee.org/Xplorehelp/#/searching-ieee-xplore/global-search) & [IEEE Xplore Search Tips](http://ieeexplore.ieee.org/Xplorehelp/#/searching-ieee-xplore/search-tips)

*Notes personnelles*

---

