# Scopus

| Fonctionnalités | Possibilités |
| :-------- | :---- |
| opérateurs<br/>booléens | `AND`<br/>`OR`<br/>`AND NOT` |
| opérateurs<br/>de proximité | `W/`*n*<br/>`PRE/`*n* |
| troncature | `*` (zéro ou plusieurs caractères)<br/>`?` (un caractère)\* <br/>`!` (zéro ou plusieurs caractères) <br/> *troncature possible à gauche, au milieu et à droite* |
| phrase | `"..."`<br/>`{...}` |
| interprétation<br/>de la requête | oui (*stemming*) |
| historique | oui |

**Exemples**   
`sensor W/15 robot` renvoie tous les documents où `sensor` se trouve à 15 mots max. de `robot`.   

`behavioral PRE/3 disturbances` renvoie tous les documents où `behavioral` précède `disturbances` de 3 mots max.

`*eat` renvoie eat, heat, meat, great, treat, wheat, etc.   
`?eat` renvoie heat, meat, etc., mais pas eat, great, treat ou wheat   
`!eat` renvoie heat, great, treat, wheat, etc., mais pas eat   
`Nure?berg` renvoie Nuremberg et Nurenberg   
`?ight` renvoie light, right, eight, fight, might, etc.   
`locom!` renvoie locomotive, locomotives, and locomotion   
`{heart-attack}` et `{heart attack}` renvoient des résultats différents.   
Idem pour `"heart-attack"` et `"heart attack"`.   
`"criminal* insan*"` renvoie criminally insane, criminal insanity, etc.

*source*: [Scopus: Access and use Support Center - Document search tips](https://service.elsevier.com/app/answers/detail/a_id/11213/supporthub/scopus/#tips)

---

*Notes personnelles*
