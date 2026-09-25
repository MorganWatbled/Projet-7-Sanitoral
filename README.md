# DWFA — Tableau de bord d'accès à l'eau potable

Mission de consulting data pour l'ONG DWFA (Drinking Water For All), visant à orienter le choix d'un pays et d'un domaine d'investissement suite à une demande de financement auprès d'un bailleur de fonds.

---

## Contexte / besoin métier

DWFA a pour ambition de donner accès à l'eau potable à tout le monde, à travers trois domaines d'expertise :
- la création de services d'accès à l'eau potable,
- la modernisation de services existants,
- le consulting auprès d'administrations/gouvernements sur les politiques d'accès à l'eau.

L'association a sollicité un financement auprès d'un bailleur de fonds sur la base de ces trois domaines. Si ce financement est accordé, il permettra d'investir dans l'un des trois domaines, dans un pays encore à déterminer.

Thibaut Renard, chef de mission, a demandé la construction d'un tableau de bord permettant de :
- identifier les pays rencontrant des difficultés d'accès à l'eau potable,
- identifier ceux sur lesquels concentrer les efforts d'investissement,

à travers des indicateurs représentatifs des trois domaines d'expertise, organisés en 3 vues (définies lors de la réunion de lancement).

## Données (source, qualité, limites)

**Sources :**
- Dataset collecté par un data engineer de DWFA, dédié à cette analyse.
- Dictionnaire des données fourni avec le jeu de données (zip).
- Sources complémentaires suggérées par Thibaut : sites de l'OMS et de la FAO pour approfondir certains indicateurs.
- Possibilité d'intégrer d'autres données complémentaires jugées pertinentes, bien que le dataset fourni soit suffisant pour une première analyse.

**Qualité :**
[À compléter : après exploration — complétude par pays, cohérence des unités et échelles entre indicateurs, année(s) de référence des données]

**Limites :**
- Le dataset est centré sur les indicateurs jugés utiles à l'analyse par le data engineer : d'éventuels indicateurs pertinents mais absents du fichier devront être recherchés via l'OMS/la FAO ou écartés faute de disponibilité.
- Le pays cible n'étant pas encore déterminé, l'analyse doit rester comparative à l'échelle de plusieurs pays plutôt que focalisée d'emblée sur un seul territoire.
[À compléter : autres limites constatées à l'exploration, ex. données manquantes pour certains pays, écarts de fraîcheur entre sources]

## Démarche (choix, outils, étapes)

1. Prise de connaissance du compte-rendu de la réunion de lancement pour identifier les 3 vues attendues et les pistes d'indicateurs déjà évoquées.
2. Sélection des indicateurs pertinents pour chacun des 3 domaines d'expertise (création, modernisation, consulting politique), à répartir sur les 3 vues.
3. Rédaction d'un **document de synthèse** présentant, pour chaque vue, les indicateurs retenus et leur justification — livrable intermédiaire à valider avant la construction du tableau de bord.
4. Réalisation, en option, d'une version basse fidélité (blueprint/mockup) du tableau de bord final, à partir des exemples fournis par Thibaut.
5. Exploration et préparation du dataset fourni par le data engineer, en s'appuyant sur le dictionnaire des données.
6. Construction du tableau de bord dans l'outil retenu, avec les 3 vues définies, en veillant à l'**accessibilité** (contrastes, lisibilité, alternatives textuelles).
7. Préparation d'une démonstration du fonctionnement du tableau de bord pour Thibaut.

**Outil :** [À compléter : Tableau (histoire Tableau partagée sur Tableau Public) ou Power BI — choix à trancher]

## Résultats + impact / recommandations

- Un document de synthèse présentant les indicateurs sélectionnés pour chacune des 3 vues, couvrant les 3 domaines d'expertise de DWFA.
- [À compléter, le cas échéant : mockup/blueprint basse fidélité du tableau de bord]
- Un tableau de bord interactif et accessible, permettant de comparer les pays sur leurs difficultés d'accès à l'eau potable.
- [À compléter : pays ou groupes de pays identifiés comme prioritaires à l'issue de l'analyse, et domaine d'expertise associé recommandé]
- **Impact attendu :** aider DWFA à orienter sa décision d'investissement (pays et domaine d'expertise) une fois le financement du bailleur de fonds confirmé.

## Limites + prochaines pistes

- L'analyse s'appuie sur un instantané de données ; une mise à jour régulière serait nécessaire si le tableau de bord doit continuer à orienter les décisions après l'attribution du financement.
- Le choix final du pays et du domaine reste une décision stratégique de DWFA : le tableau de bord fournit un support d'aide à la décision, pas une décision automatisée.
[À compléter : pistes complémentaires, ex. enrichissement avec des données OMS/FAO plus récentes ou plus granulaires, ajout d'indicateurs socio-économiques]

---

*Projet réalisé dans le cadre de la mission consultant Data Analyst pour l'ONG DWFA (Drinking Water For All), sous la responsabilité de Thibaut Renard, chef de mission.*
