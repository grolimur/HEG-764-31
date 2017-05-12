# Scopus

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | AND<br/>OR<br/>AND NOT |
| opérateurs<br/>de proximité | W/*n*<br/>PRE/*n* |
| troncature | * (zéro ou plusieurs caractères)<br/>? (un caractère exactement)\* <br/>! (zéro ou plusieurs caractères) <br/> *troncature possible à gauche, au milieu et à droite* |
| phrase | "..."<br/>{...} |
| interprétation<br/>de la requête | oui (*stemming* et variantes UK/US) |
| historique | oui |

**Exemples**   
`*eat` renvoie eat, heat, meat, great, treat, wheat, etc.   
`?eat` renvoie heat, meat, etc., mais pas eat, great, treat ou wheat   
`!eat` renvoie heat, great, treat, wheat, etc., mais pas eat   
`Nure?berg` renvoie Nuremberg et Nurenberg   
`?ight` renvoie light, right, eight, fight, might, etc.   
`locom!` renvoie locomotive, locomotives, and locomotion   



`pain W/15 morphine` renvoie les résultats où "pain" se trouve à max. 15 mots de "morphine".   
*behavioural **PRE/3** disturbances* renvoie les résultats où "behavioural" précède "disturbances"de 3 mots max.   

**h*rt** renvoie hurt, heart, etc.   
**transplant??** renvoie transplanted et transplanter.   
**"heart attack"** est équivalent à **"heart-attack"**, car le tiret est ignoré.   
**"criminal* insane"** renvoie "criminally insane", etc.   
**{heart-attack}** est différent de **{heart attack}**, car le tiret est pris en compte.   
**{health care?}** renvoie tous les résultats du type "health care...".   

*source*: [Scopus: Access and use Support Center - Document search tips](https://service.elsevier.com/app/answers/detail/a_id/11213/supporthub/scopus/#tips)

