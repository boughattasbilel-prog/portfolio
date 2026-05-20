# Auto-Cadreuse Project — ISSAT Sousse

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

![Machine Cross-Section](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/49ebede2-baa9-4a49-9b07-7529d2bc41d4.png)
![Winding Machine White BG](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/7f82a85a-284b-4d30-b3b1-bcd8e9357c30.png)
![Vue de dessus schématique](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/fc292dc6-056c-4816-a44e-2d1d9656c2fd.png)
![Schéma cinématique simplifié](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/6beefa33-bb07-418d-8de0-858a8a78314c.png)
![Organigramme du programme de contrôle](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/6fdd4efb-3482-42d7-b89f-85a62387f2aa.png)




