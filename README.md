Ce projet consiste à construire un modèle de prédiction pour déterminer si un emprunteur remboursera son prêt ou non, en utilisant un sous-ensemble de données provenant de LendingClub. Voici un résumé des principales étapes du projet :

   ## Objectif et Données : 
   L'objectif est de créer un modèle de prédiction pour déterminer si un emprunteur remboursera son prêt. Les données proviennent de LendingClub, une plateforme de prêt entre pairs. Les données contiennent des informations sur les caractéristiques des emprunteurs et l'état de remboursement des prêts.

   ## Analyse Exploratoire des Données (EDA) : 
   Cette section vise à comprendre les données en effectuant des analyses statistiques et visuelles. On a examiné la distribution des états de prêt, l'impact du montant du prêt, les corrélations entre variables continues, et des visualisations basées sur des features telles que le grade, la durée de l'emploi, etc.

   ## Pré-traitement des Données : Dans cette section, plusieurs étapes ont été réalisées :
        Suppression des colonnes non informatives ou comportant des données manquantes.
        Remplissage des valeurs manquantes dans certaines colonnes en fonction de valeurs existantes.
        Conversion des variables catégorielles en variables binaires (variables dummies).

##    Répartition Entraînement / Test : 
Les données ont été divisées en ensembles d'entraînement et de test à l'aide de la fonction train_test_split de Scikit-Learn.

 ##   Normalisation des Données :
 Les features ont été normalisées à l'aide de la mise à l'échelle MinMaxScaler pour mettre toutes les valeurs dans une plage commune.

  ##  Création du Modèle :
  Un modèle de réseau neuronal séquentiel a été construit en utilisant TensorFlow et Keras. Le modèle comporte plusieurs couches denses et utilise la fonction d'activation ReLU. La couche de sortie utilise une fonction d'activation sigmoid pour prédire la probabilité de remboursement du prêt.

  ##  Entraînement du Modèle : 
  Le modèle a été entraîné sur les données d'entraînement à l'aide de la méthode fit. Les données de validation ont été utilisées pour évaluer les performances pendant l'entraînement.

 ##   Évaluation de la Performance : 
 La performance du modèle a été évaluée en utilisant le jeu de test. On a affiché la perte d'entraînement et de validation au fil des époques. De plus, on a généré un rapport de classification et une matrice de confusion pour évaluer la capacité du modèle à prédire les remboursements.

En fin de compte, ce projet a permis de construire et d'évaluer un modèle de prédiction de remboursement de prêt en utilisant des données historiques de LendingClub. Le modèle peut être utilisé pour évaluer le risque de non-remboursement des prêts futurs.


# Jean-Baptiste TOHOUEGNON
