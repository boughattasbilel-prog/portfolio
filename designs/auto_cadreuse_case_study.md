# Confidential Auto-Cadreuse Project — ISSAT Sousse

> **Note académique :** Ce case study est intentionnellement présenté dans une version portfolio publique. Aucune donnée industrielle propriétaire, numéro de pièce interne, dimension exacte confidentielle ou résultat de validation non publié n'est divulgué. Tous les visuels sont des croquis originaux dessinés à la main ou des représentations simplifiées créées indépendamment à des fins de portfolio.

---

## Vue d'ensemble du projet

**Établissement :** ISSAT Sousse — Institut Supérieur des Sciences Appliquées et de Technologie
**Type :** Projet de Fin d'Études (PFE) — Licence Appliquée, Génie Mécanique
**Intitulé :** *"Programmation et automatisation d'une machine de façonnage de fer à béton"*
**Encadreur :** Mr. Louhichi Borhen

### Objectif

Concevoir et développer une **machine cadreuse automatique compacte et programmable** capable d'exécuter le cycle complet de fabrication des cadres d'armature en acier pour la construction en béton armé.

**Cibles principales :**
- Automatiser les opérations de dressage, avance, façonnage et coupe pour des barres acier ⌀ 6, 8 et 10 mm
- Atteindre un angle de pliage de 0° à 180° en 1 seconde (acier Re = 500 MPa)
- Supporter la programmation de plusieurs formes de cadres (carré, rectangulaire, personnalisé)
- Respecter des contraintes d'encombrement strict : L ≤ 0,5 m / l ≤ 0,7 m / h ≤ 0,5 m / Masse ≤ 70 kg
- Maintenir la fabricabilité pour un usage atelier à faible coût (≤ 5 000 DT)

**Livrable :** Un concept de machine validé par calculs mécaniques, modélisation 3D et programme de contrôle — présenté dans un format légal et adapté au portfolio.

---

## Ce que j'ai fait

- Réalisé l'**analyse fonctionnelle complète** du système : modélisation FAST, Bête à cornes, Diagramme Pieuvre — identification des fonctions de service et des contraintes
- Conduit une **sélection multi-critères des solutions technologiques** (tri croisé) pour chaque sous-système : façonnage, coupe, avance, guidage
- Effectué le **dimensionnement mécanique complet** : réducteurs de vitesse, arbres (calcul RDM torsion + flexion), roulements (calcul statique et dynamique)
- Réalisé le **calcul et la sélection des moteurs pas à pas** pour les 3 axes — validés par les couples requis issus des caractéristiques mécaniques de l'acier
- Produit le **dossier de conception 3D complet sous SolidWorks** : 9 pièces fonctionnelles modélisées, 4 sous-systèmes assemblés, vues éclatées et vues en perspective
- Développé le **programme de contrôle complet en Python** sur Raspberry Pi — 3 modes opérationnels (AutoMode, AutoProg, Manuel), interface LCD + clavier matriciel, pilotage des 3 moteurs via GPIO
- Aligné le concept avec les **normes de façonnage** NF EN 1992-1-1 et NF A 35-027

---

## Outils & Méthodes

| Outil / Méthode | Utilisation |
|---|---|
| **SolidWorks** | Modélisation 3D complète — pièces, assemblages, vues éclatées |
| **Python** | Programme de contrôle V1.0 — 3 modes, GPIO, LCD, clavier matriciel |
| **Raspberry Pi (Raspbian)** | Architecture de commande — microcontrôleur principal |
| **RDM (Résistance des Matériaux)** | Dimensionnement arbre — torsion + flexion combinées |
| **Analyse fonctionnelle (FAST / Pieuvre)** | Décomposition et cartographie des fonctions de service |
| **Tri croisé multi-critères** | Sélection optimale des solutions technologiques |
| **Catalogue SKF** | Sélection et validation des roulements |
| **Normes NF EN 1992-1-1 / NF A 35-027** | Respect des tolérances et conditions de façonnage acier |
| **Schémas cinématiques** | Validation des chaînes de transmission (façonnage + avance + coupe) |

---

## Défi d'ingénierie

Le défi central était de **concentrer 3 systèmes mécaniques distincts** — façonnage, coupe et avance — dans une enveloppe machine compacte (≤ 0,5 × 0,7 × 0,5 m) tout en garantissant la précision angulaire et dimensionnelle exigée par les normes de façonnage acier.

Le système de façonnage imposait un rapport de réduction élevé pour contrôler précisément l'angle de pliage — la barre doit être pliée sans rebond ni déformation parasite. Simultanément, le système de coupe devait générer une force suffisante pour cisailler une barre ⌀ 10 mm, exigeant une conversion rotation → translation par vis-écrou soigneusement dimensionnée.

Sur le plan logiciel, la synchronisation des 3 moteurs en séquence — avance mesurée → pliage angulaire → coupe — avec une interface opérateur simple (clavier + LCD) représentait un véritable défi d'intégration système.

---

## Résultats

- ✅ Machine cadreuse compacte conçue et validée par calculs mécaniques complets
- ✅ Rapport de réduction façonnage et coupe dimensionnés et validés par calcul de couple
- ✅ Diamètre d'arbre déterminé par RDM sous sollicitations combinées torsion + flexion
- ✅ Roulements sélectionnés et validés — durée de vie statique et dynamique calculées
- ✅ Dossier de conception 3D complet sous SolidWorks — 9 pièces fonctionnelles modélisées
- ✅ Programme Python V1.0 opérationnel — 3 modes de fonctionnement fonctionnels
- ✅ Enveloppe machine, masse et cible de coût respectées

---

## Médias du projet

> Tous les visuels ci-dessous sont des **croquis originaux dessinés à la main** ou des **représentations simplifiées** créées indépendamment à des fins de portfolio. Aucune donnée CAO confidentielle n'est montrée.

- Croquis de l'architecture globale de la machine (vue de dessus schématique)
- Schéma cinématique simplifié — chaîne de transmission façonnage + avance
- Esquisse des 4 sous-systèmes annotée (carcasse, façonnage, coupe, avance)
- Organigramme simplifié du programme de contrôle (AutoMode / AutoProg / Manuel)

---

## Ce qu'il ne faut PAS publier

| ❌ Ne pas divulguer | ✅ Sécurisé à dire |
|---|---|
| Fichiers CAO internes ou plans détaillés | "Modélisé sous SolidWorks — 9 pièces fonctionnelles" |
| Valeurs de dimensionnement exactes | "Dimensionnement arbre par RDM sous torsion + flexion" |
| Code source complet du programme | "Programme Python V1.0 — 3 modes opérationnels" |
| Résultats de calcul numériques détaillés | "Roulements sélectionnés et validés par calcul dynamique" |
| Plans de fabrication ou cotes | "Conception respectant les normes NF EN 1992-1-1" |

---

*Dernière mise à jour : Mai 2026 — Version portfolio*
