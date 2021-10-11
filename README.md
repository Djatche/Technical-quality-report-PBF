# Rapport supervision qualité technique.


## Description du projet.
Ce dépôt contient du code pour analyser les données de supervision qualité technique des formations sanitaires du district de santé de YOKO dans la région du centre Cameroon. Le fichier csv est téléchargé de la plateforme du projet PBF. Ces données ont été obtenues de la supervision de 15 formations sanitaires à l'aide d'une grille de supervision. Cette dernière d'une vingtaine de pages, contient des questions (indicateurs) au nombre de 197 réparties en 19 catégories. Une copie de cette grille se retrouve dans le repertoire Documentation du dépôt.

Liste des différentes catégories contenues dans la grille de supervision (collecte de données):                
Indicateurs généraux    
Business plan trimestriel   
Partie financière   
Hygiène et stérilisation    
Consultation externe     
Planification familiale
Laboratoire   
Salle d'hospitalisation   
Gestion de médicaments   
Médicaments traceurs   
Maternité   
Petite chirurgie      
Tuberculose     
Vaccination    
Consultation prénatale    
Lutte contre le VIH    
PBF Communautaire   
Malnutrition   
Etat civil



## Le plan d'analyse des données.

### Questions

Quelle est la tendance des scores de différentes catégories pour chaque formation sanitaire trimestre après trimestre le long des années 2019, 2020, 2021.    
Cette tendance est représentée par un graphique linéaire avec les scores en ordonnée et les trimestres en abcisse. Sur le même graphique, on retrouve 3 courbes dont une pour chaque année

Quelle est la performance du trimestre 2 de 2021 d'une formation santaire pour chaque categorie ainsi que son rang au sein du district par rapport autres formations sanitaires d'une part et part rapport au score maximum de cette catégorie et au score moyen du district d'autre part.        
Ce ranking est représenté par un graphique en barre avec les formations sanitaires classées par ordre décroissant. Le score maximal et le score moyen du district sont représentés avec une couleur différente.

Quelles sont les limites des données (qualité) en terme de données manquantes et de données aberrantes.


### Les librairies utlisées.
Matplotlib    
Pandas       
Numpy      
Seaborn    

### Les fichiers disponibles dans ce dépôt      
- data/: données extraite de la plateforme dhis2 du projet pbf sous forme de fichier csv **'score_qualite_T2_2021.csv'**
- documentation/: **'Grille_PMA_qualite_PBF.pdf'** et **'Rapport_qualite_final_Q2_2021_DS_YOKO'** respectivement fiche de collecte de données sous forme de check list et le rapport d'évaluation qualité.        
- images/:
    - Missing_values/:
    **'heatmap_missing_value.png'** qui est un fichier qui repertorie les données manquantes dans un dataframe
    - Performance_evolution/: 
    **'business_plan.png'** fichier image du graphique représentant l'évolution du score business plan trimestre après trimestre. ON note trois courbes pour les années 2019, 2020 et les 2 premiers trimestre 2021. Toutes les 15 formations sanitaires sont représentées dans le graphique.
    - Ranking/:
    **'ranking_business_plan'** fichier image du diagramme en barre de performances (scores) de la catégorie "business plan". Les formations sanitaires sont classées dans le graphique par ordre décroissant. Du plus performant au moins. A noter que le score maximal de la catégorie et le score moyen du district pour cette catégorie ont été représenté par une couleur différente dans ce diagramme en barre.
- **'pbf_dict_columns.py'**: fichier python qui contient un dictionnaire avec comme clés les noms actuels des colonnes (indicateurs) et comme valeurs les noms plus courts des colonnes désirés.
- **'quality_score_pbf.ipynb'**: fichier notebook qui contient le code pour l'analyse des données.

