# IEEE Xplore

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*<br/>ONEAR/*n* |
| troncature | gauche - milieu - droite<br/>* (zéro à cinq caractères) |
| phrase | "..." |
| interpréation<br/>de la requête | stemming<br/>variantes UK/US |
| historique | oui |

**Exemples**   
*implantable **NEAR/3** cardiac* renvoie les résultats où "implantable" se trouve à max. 3 mots de "cardiac".   
*implantable **ONEAR/3** cardiac* renvoie les résultats où "implantable" précède "cardiac" de 3 mots max.   

**electro*** renvoie electron, electrons, electronic, electronics, electromagnetic, electromechanical, electrostatic, etc.   
***optic** renvoie optic,fiber-optic, electrooptic, acoustooptic, etc.   
**me*n** renvoie men, mean, median, etc.   
