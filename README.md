
# Analyse des Effets des Prix des Matières Premières sur les Secteurs S&P

Ce projet vise à modéliser et analyser les relations entre l'évolution des prix des matières premières et les performances de trois secteurs économiques majeurs (financier, technologique, immobilier) représentés par des indices S&P. L'objectif est de mieux comprendre les interactions entre ces variables à l'aide de techniques économétriques avancées, incluant la modélisation univariée et multivariée.

## Objectifs du Projet

1. Identifier les relations dynamiques entre les prix des matières premières et les performances des secteurs.
2. Évaluer l'impact des variations saisonnières et des chocs exogènes.
3. Appliquer des modèles économétriques pour estimer les causalités, prédictions, et réponses aux chocs.

## Approche Méthodologique

### **1. Modélisation Univariée**

Dans cette première étape, chaque série temporelle est analysée individuellement :

1. **Choix des Séries** : 
   - Prix des matières premières (indice Bloomberg Commodity Index).
   - Indices sectoriels : S&P Financials, S&P Information Technology, S&P Real Estate.
   
2. **Analyse Préliminaire** :
   - Représentations graphiques et autocorrélogrammes (simples et partiels).
   - Tests de stationnarité (ADF, KPSS) pour détecter les racines unitaires.
   
3. **Modèle ARMA** :
   - Ajustement d'un modèle ARMA pour une des séries.
   - Validation des conditions d'adéquation.

4. **Prédictions** :
   - Prévisions sur des horizons de 1 à 3 périodes.
   - Comparaison des séries initiales non stationnarisées et stationnarisées.

---

### **2. Modélisation Multivariée**

Dans cette deuxième étape, toutes les séries stationnarisées sont intégrées dans un cadre multivarié pour explorer leurs interactions :

1. **Modèle VAR** :
   - Estimation d'un modèle VAR avec sélection du nombre optimal de retards.
   - Analyse de la cohérence des résultats par rapport aux attentes économiques.

2. **Relations de Causalité** :
   - Test de causalité de Granger pour identifier les relations directionnelles entre les séries.

3. **Analyse des Réponses aux Chocs** :
   - Analyse impulsion-réponse des chocs via :
     - Modèles VAR.
     - Projections locales.
   - Justification du choix de l'ordre des variables via la décomposition de Choleski.

4. **Test de Cointégration** :
   - Test de Johansen pour vérifier l'existence de relations de long terme.
   - Modèle VECM si nécessaire pour intégrer les relations à long terme.

---

## Données et Période

- **Période couverte** : Octobre 2001 à Décembre 2023 (observations mensuelles).
- **Séries étudiées** :
  - Indice Bloomberg Commodity Index (BCOM).
  - S&P Financials Select Sector (S5FINL).
  - S&P Information Technology (S5INFT).
  - S&P Real Estate (S5RLST).

## Résultats Attendus

- Identification des causalités directes entre les fluctuations des matières premières et les performances sectorielles.
- Évaluation de la sensibilité de chaque secteur aux variations des prix des matières premières.

