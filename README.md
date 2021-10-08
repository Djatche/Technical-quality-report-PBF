# Rapport supervision qualité technique.


## Description du projet.
Ce dépôt contient du code pour analyser les données de supervision qualité technique des formations sanitaires du district de santé de YOKO dans la région du centre Cameroon. Le fichier csv est téléchargé de la plateforme du projet PBF. Ces données ont été obtenues de la supervision de 15 formations sanitaires à l'aide d'une grille de supervision. Cette dernière d'une vingtaine de pages, contient des questions (indicateurs) réparties en 19 catégories. Une copie se retrouve dans le repertoire Documentation du dépôt.



## Le plan d'analyse des données.

### Questions

Quelle est la tendance des scores de différentes catégories pour chaque formation sanitaire trimestre après trimestre le long des années 2019, 2020, 2021. Cette tendance est représentée par un graphique linéaire avec les coûts en ordonnées et les trimestres en abcisses. Sur le même graphique, 3 courbes dont une pour chaque année

Quelle est la performance du trimestre 2 2021 d'une formation santaire pour chaque categories ainsi que son rang au sen du district par rapport autres formations sanitaires d'une part et part rapport au score maximum de cette catégorie et au score moyen du district d'autre part. Ce ranking est représenté par un graphique en barres avec les formations sanitaires classées par ordre décroissant. Le score maximal et le score moyen du district sont représentés avec une couleur différente.

Quelles sont les limites des données (qualité) en terme de données manquantes et de données aberrantes.


### Les librairies utlisées.
Matplotlib    
Pandas       
Numpy      
Seaborn     