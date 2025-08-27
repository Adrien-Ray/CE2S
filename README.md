# README

 - [doc technico-fonctionnel : DAT](./doc/DAT.md)
 - [doc technico-fonctionnel : cycle générale de fonctionnement](./doc/sequence_general.md)
 - [doc technico-fonctionnel : modèle de donnée](./doc/datamodel.md)


## réflexions production / entretiens

note: a chaque tour on retire 60 points puis on ajoute max 30 nourriture et 30 logement

### food

calcul pour prod repas avec économie d'échelle (fonction nbr employés)

heures par employer 120 * nbr employer + boss * coef(1 + (0.1 * nbr employers)) -> arrondi entier inférieur

une inflation des salaires forcera à bouger les prix, forçant l'inflation des salaires

### logement

5 type de logements

||SDF|6.25m2|12.5m2|25m2|50m2|100m2|
|-|-|-|-|-|-|-|
|ajout PV|0|10|20|25|28|30|
|heures travail construction|0|120|240|480|960|1920|
|nbr plein temp construction|0|1|2|4|8|16|
|restoration (heures) (nécessaire à chaque tour)|0|12|24|48|96|192|