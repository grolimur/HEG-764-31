# Engineering Village

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | `AND`<br/>`OR`<br/>`NOT` |
| opérateurs<br/>de proximité | `NEAR/`*n*<br/>`ONEAR/`*n*  |
| troncature | `*` (zéro ou plus de caractères)<br/>`?` (un caractère)<br/>`$` (variations du terme)<br/>*troncature possible à gauche, au milieu et à droite* |
| phrase | `"..."`<br/>`{...}` |
| interprétation<br/>de la requête | oui (*autostemming*) |
| historique | oui |

**Exemples**   
`laser NEAR/4 diode` renvoie les résultats où "laser" se trouve à max. 4 mots de "diode" (avant ou après).   
`laser ONEAR/5 diode` renvoie les résultats où "laser" précède "diode" de 5 mots max.   

`comput*` renvoie computer, computers, computerize, computerization, etc.   
`sul*ate` renvoie sulphate et sulfate.   
`*sorption` renvoie adsorption, absorption, resorption, etc.   
`wom?n` renvoie woman et women.   
`t??th` renvoie tooth, teeth, truth, tenth, etc.   
`$management` renvoie manage, managed, manager, managers, managing, management, etc.   

*source*: [Engineering Village: Access and Use Support Center](https://service.elsevier.com/app/home/supporthub/engineering-village/)

*Notes personnelles*

---
