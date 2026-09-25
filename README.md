# Sanitoral — Tableau de bord de suivi de projets (Power BI)

Mission de visualisation de données réalisée en tant que consultant Data Analyst chez ESN Data, déployé chez le client Sanitoral, société internationale de soins bucco-dentaires.

---

## Contexte / besoin métier

Le service Project Management Office de Sanitoral, piloté par Sophie, cheffe de projet, a besoin d'un tableau de bord pour suivre l'avancement des projets et leurs coûts, identifier les retards, et contrôler les performances afin que l'équipe puisse engager les actions correctives adéquates.

La démarche a été formalisée dans un **Product Strategy Canvas** (modèle ESN Data), validé par Sophie :
- **Nom du tableau de bord** : *Pilotage des projets – Vue hiérarchique Groupe / Région / Pays*
- **Objectif** : établir un ordre hiérarchique de lecture, du niveau groupe jusqu'au niveau pays.
- **Utilisateurs et user stories identifiés** :
  - **Directeur général** — être informé des données par région pour identifier les régions en difficulté et échanger avec les directeurs régionaux en cas d'alerte ; visualiser les performances de coûts, délais et avancement par région.
  - **Directeur régional** — être informé des données par pays et identifier les pays en difficulté ; comparer les indices de performance de ses pays et identifier les écarts ; accéder au détail des projets d'un pays sélectionné pour analyser la situation.
  - **Directeur de pays** — être informé des données par projet en cas de problème et accéder directement au détail des projets ; suivre l'avancement et les indicateurs clés par projet pour anticiper les risques ; identifier rapidement les projets en alerte pour mettre en place des actions.

## Données (source, qualité, limites)

**Sources :** jeu de données extrait du logiciel de gestion de projets de Sanitoral (projets entre 2018 et début 2022), accompagné d'un dictionnaire des données.

**Qualité :** les données brutes nécessitaient un nettoyage avant intégration : colonnes inutilisables pour l'analyse supprimées, lignes en doublon supprimées, valeurs négatives (incohérentes pour des indicateurs comme les coûts ou délais) supprimées.

**Limites :**
- Le nettoyage a été réalisé manuellement dans cette phase ; l'automatisation complète via Power Query Editor (pour la mise à jour hebdomadaire souhaitée par Sophie) reste à finaliser/documenter dans l'onglet dédié du tableau de bord.
- Les données s'arrêtent début 2022 : pas de visibilité sur les projets plus récents dans le jeu de données initial.

## Démarche (choix, outils, étapes)

1. Réunion de cadrage avec Sophie, note de cadrage, puis formalisation du Product Strategy Canvas (utilisateurs, user stories, objectif du tableau de bord).
2. Validation du Product Strategy Canvas par le mentor puis par Sophie, avant tout développement.
3. Nettoyage des données : suppression des colonnes inexploitables, des doublons et des valeurs négatives, puis structuration de la base de données.
4. Modélisation des données récupérées du fichier Excel sous forme de tables, chargées et reliées dans **Power BI**.
5. Construction du tableau de bord avec **3 pages**, une par persona identifié dans le Product Strategy Canvas : *Directeur Général*, *Directeur Régional*, *Directeur Pays* — permettant à chaque niveau hiérarchique de repérer d'où vient un problème.
6. Création d'une table dédiée pour construire un **diagramme de Gantt**, permettant de visualiser et planifier les projets dans le temps.
7. Mise en forme d'un onglet de documentation (Product Strategy Canvas, procédure de mise à jour, modèle de données) au sein du tableau de bord.

**Outil :** Power BI.

## Résultats + impact / recommandations

- Un Product Strategy Canvas validé, structurant le tableau de bord autour de 3 profils utilisateurs et de leur besoin propre (vision groupe, vision région, vision projet).
- Un tableau de bord Power BI opérationnel avec **3 pages dédiées** (Directeur Général, Directeur Régional, Directeur Pays), permettant une lecture hiérarchique cohérente avec la demande initiale.
- Un diagramme de Gantt intégré pour la planification et le suivi temporel des projets.
- **Impact attendu :** donner à chaque niveau de management chez Sanitoral (du directeur général au directeur de pays) une vue adaptée à son périmètre de décision, pour repérer rapidement l'origine d'un problème et agir avant que les retards ou dérives de coûts ne s'aggravent.

## Limites + prochaines pistes

- Le tableau de bord repose sur un historique 2018-début 2022 ; sa pertinence à long terme dépendra de la mise en place effective de l'automatisation Power Query pour les mises à jour hebdomadaires.
- L'onglet de documentation (procédure de mise à jour, modèle de données) doit encore être complété pour que Sanitoral puisse gérer les futures mises à jour en autonomie, comme demandé par Sophie.
- Une extension du diagramme de Gantt avec des alertes visuelles automatiques (retards, dépassements budgétaires) pourrait renforcer l'usage par les directeurs de pays au quotidien.

---

*Projet réalisé dans le cadre de la mission consultant Data Analyst d'ESN Data pour le client Sanitoral, en lien avec Sophie, cheffe de projet PMO.*
