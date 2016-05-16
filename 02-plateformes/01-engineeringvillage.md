# Engineering Village

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>NOT |
| opérateurs<br/>de proximité | NEAR/*n*<br/>ONEAR/*n*  |
| troncature | gauche - milieu - droite<br/>* (zéro ou plus de caractères)<br/>? (un caractère)<br/>$ (variations) |
| phrase | "..."<br/>{...} |
| interpréation<br/>de la requête | autostemming |
| historique | oui |

**Exemples**   
*laser **NEAR/4** diode* renvoie les résultats où "laser" se trouve à max. 3 mots de "diode".   
*laser **ONEAR/5** diode* renvoie les résultats où "laser" précède "diode" de 3 mots max.   

**comput*** renvoie computer, computers, computerize, computerization, etc.   
**sul*ate** renvoie sulphate et sulfate.   
***sorption** renvoie adsorption, absorption, resorption, etc.   
**wom?n** renvoie woman et women.   
**t??th** renvoie tooth, teeth, truth, tenth, etc.   
**$management** renvoie manage, managed, manager, managers, managing, management, etc.   

